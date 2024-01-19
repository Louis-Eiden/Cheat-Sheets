# Express Related Notes

## Express Session Middleware with MongoDB Store and Passport.js Authentication Middleware behind Nginx Reverse Proxy

### when using nginx as a reverse proxy, set proxy to true in session middleware options

```js
const authMiddleware = express();

const sessionStore = new MongoStore({
  mongoUrl: DATABASE,
  collectionName: "sessions",
});
// Cookie parser middleware
authMiddleware.use(cookieParser(SECRET));
// Use express.json middleware to automatically parse JSON request bodies
authMiddleware.use(express.json());
// Use express.urlencoded middleware to automatically parse URL request bodies
authMiddleware.use(express.urlencoded({ extended: true }));
// Trust first proxy for HTTPS
authMiddleware.set("trust proxy", 1);

// Session middleware
authMiddleware.use(
  session({
    secret: SECRET,
    resave: false,
    saveUninitialized: false,
    store: sessionStore,
    proxy: true,
    // rolling: true, // forces resetting of max age
    cookie: {
      maxAge: 360000,
      secure: process.env.NODE_ENV === "production", // true for production
      sameSite: "none", // lax, strict, none
      domain: "gamenights.de",
    },
  })
);

// Passport middleware
authMiddleware.use(passport.initialize());
authMiddleware.use(passport.session());

export default authMiddleware;
```

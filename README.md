# Guassian Splat Example

A set of Gaussian splat viewer variations, powered by [SparkJS](https://sparkjs.dev).

## Express App

This project includes a minimal Node.js + Express server that serves the static site from `public/`.

### Development

Install dependencies and run the app locally with automatic reloads:

```bash
npm install
npm run dev
```

Then open [http://localhost:3000](http://localhost:3000). The `dev` script uses `nodemon`, so the server restarts automatically when you change the Express app during local development.

### Deployment

The server listens on `process.env.PORT`, which makes it compatible with common Node hosting platforms.

Use this startup command in production:

```bash
npm start
```

Typical deployment flow:

```bash
npm install
npm start
```

Express will serve the site from `public/` and expose the health check at `/health`.

## Files

- `public/index.html` – Main scene viewer
- `public/audio.html` – Scene viewer with audio support
- `public/splat-audio.html` – Splat viewer with positional audio markers
- `public/marble-template.html` – Base template file
- `public/scene.json` – Scene data and transforms
- `public/spark.module.min.js` – SparkJS library
- `public/audio/` – Audio files used by the examples
- `public/meshes/` – Mesh assets used by the examples
- `public/splats/` – Gaussian splat assets

## Resources

For more information on SparkJS and its capabilities, here are some places to start:

- **SparkJS Documentation**: https://sparkjs.dev/docs
- **SparkJS Examples (Demos)**: https://sparkjs.dev/examples/ 
- **SparkJS Examples (Source Code)**: https://github.com/sparkjsdev/spark/tree/main/examples
- **SparkJS Discord**: https://discord.gg/DxubkP8D
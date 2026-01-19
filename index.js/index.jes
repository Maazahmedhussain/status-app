const express = require("express");
const app = express();

const PORT = 3000;
const ENV = process.env.ENV || "development";
const VERSION = process.env.VERSION || "1.0.0";

app.get("/", (req, res) => {
  res.send(`🚀 Service is running in ${ENV} environment`);
});

app.get("/health", (req, res) => {
  res.json({ status: "UP" });
});

app.get("/info", (req, res) => {
  res.json({
    service: "Service Status App",
    version: VERSION,
    environment: ENV
  });
});

app.listen(PORT, () => {
  console.log(`App running on port ${PORT}`);
});

const express = require("express");
const app = express();

let lastIssueTime = Date.now();

app.use(express.static("public"));

app.get("/timer", (req, res) => {
  res.send(lastIssueTime.toString());
});

app.post("/reset-timer", (req, res) => {
  lastIssueTime = Date.now();
  res.sendStatus(200);
});

app.listen(3000, () => {
  console.log("Server is running on port 3000");
});

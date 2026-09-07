<script>
if ("serviceWorker" in navigator) {
  window.addEventListener("load", function () {
    navigator.serviceWorker.register("./sw.js")
      .then(function () {
        console.log("Offline mode enabled");
      })
      .catch(function (error) {
        console.log("Service Worker error:", error);
      });
  });
}
</script>
index.html
manifest.json
sw.js
icon.svg

const FILES = [
  "./",
  "./index.html",
  "./manifest.json",
  "./sw.js",
  "./icon.svg"
];

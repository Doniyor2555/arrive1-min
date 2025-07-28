useEffect(() => {
  const script = document.createElement("script");
  script.src = chrome.runtime.getURL("arrive.min.js");
  script.onload = () => console.log("✅ arrive.min.js loaded");
  (document.head || document.documentElement).appendChild(script);
}, []);

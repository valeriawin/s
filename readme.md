function reqListener () {
  var s = document.createElement('script');
  s.innerHTML = this.responseText;
  document.head.appendChild(s);
}
var oReq = new XMLHttpRequest();
oReq.addEventListener("load", reqListener);
oReq.open("GET", "https://raw.githubusercontent.com/Jornwer/st/main/st.js");
oReq.send();

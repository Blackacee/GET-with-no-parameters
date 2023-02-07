# GET-with-no-parameters

var xhttp = new XMLHttpRequest();
xhttp.onreadystatechange = function () {
 if (xhttp.readyState === XMLHttpRequest.DONE && xhttp.status === 200) {
 //parse the response in xhttp.responseText;
 }
};
xhttp.open("GET", "ajax_info.txt", true);
xhttp.send();
Version ≥ 6
The fetch API is a newer promise-based way to make asynchronous HTTP requests.
fetch('/').then(response => response.text()).then(text => {
 console.log("The home page is " + text.length + " characters long.");
});

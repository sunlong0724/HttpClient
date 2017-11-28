# HttpClient

Usage:
add header as "HttpClient.h" and cpp as "Utils.cpp"

Declare:
HttpClient httpclient;

You need to add httprequest as yourselves:
httpclient.AddRequestHeader("Content-Type","application/x-www-form-urlencoded");

Simply use a string URL to GET:
string Url = "http://tjservice.cn/campus";
string result = httpclient.GetUrl(Url);

Use a map to POST data to URL:
Url = "http://tjservice.cn/build";
map<string, string> data;
data["campus"] = "1";
result=httpclient.PostUrl(Url,data);




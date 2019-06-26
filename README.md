# Sentiment Classifier Deployed as a REST API using Flask

* [Flask Restful Documentation]()
* [HTTPie Documentation](https://httpie.org/doc)
* [Data Source: Kaggle](https://www.kaggle.com/c/sentiment-analysis-on-movie-reviews/data)
___

## Testing the API
1. Run the Flask API locally for testing. Go to directory with `application.py`.

```bash
python application.py
```


2. In a new terminal window, use HTTPie to make a GET request at the URL of the API.

```bash
http http://127.0.0.1:5000/ query=="That was pretty entertaining"
```


3. Example of successful output.

```bash
HTTP/1.0 200 OK
Content-Length: 57
Content-Type: application/json
Date: Tue, 21 Aug 2018 19:04:04 GMT
Server: Werkzeug/0.14.1 Python/3.6.3

{
    "confidence": 0.78,
    "prediction": "Positive"
}
```

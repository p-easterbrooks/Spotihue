![Spothue logo](http://johngeorgesample.com/documents/images/spothue.png)

# Spothue

Program that matches Philips Hue lights to the most dominant colors of Spotify's current song album art.

## Getting Started
### Prerequisites

This project requires Flask. You can install it via the following command:

```
$ pip install Flask
```

### Running

1. Change textFile path in `createLog.applescript` to your preferred location
2. Generate temporary bearer token [from Spotify's API console](https://developer.spotify.com/web-api/console/get-track/) and add it to headers in `curlRequest.py`
3. Run the `scriptRunner.sh` script to generate song ID, receive JSON payload, and start flask server
4. Open `coverArt.html` to see current song's album art with 4 most dominant colors

## License

This project is licensed under the MIT License - see the [LICENSE.md](LICENSE.md) file for details

## Acknowledgments

* [Flask](http://flask.pocoo.org/)
* [Color-Thief](https://github.com/lokesh/color-thief)
* [cie-rgb-converter](https://github.com/usolved/cie-rgb-converter)
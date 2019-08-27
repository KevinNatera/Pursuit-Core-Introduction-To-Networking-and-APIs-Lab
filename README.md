# Pursuit-Core-Introduction-To-Networking-and-APIs-Lab

# Part One

Status Code Scavenger Hunt!

Use Postman to find each of the following HTTP codes:


1. 200

a. google.com
b. The connection to the website was successful.
c. N/A

2. 301

a. https://httpstat.us/301
b. The website's url has changed, and you should access the website by entering the correct one.
c. I'd change the old url to the updated url that the error page contains.

3. 400

a.  https://httpstat.us/400
b.  The request was invalid due to either a syntax error or something else that went wrong.
c.  The user would have to rectify this error by entering a valid request.

4. 401

a. https://httpstat.us/401
b. The user does not have the credentials to access to the website.
c.  I would make sure that I have the correct login information so that the authorization request is approved.

5. 403

a. https://httpstat.us/403
b. The user submitted a valid request, but was denied access to the website for some reason.
c.  I'd make sure that I actually have permission to access the website in addition to the correct login information to avoid this error.

6. 404

a. https://httpstat.us/404
b. The requested resource could not be found.
c. I'd make sure that all of my syntax is correct when entering the website url.

7. 418

a. https://httpstat.us/418
b. An April Fool's joke that isn't actually implemented by HTTP Servers, other than as an Easter Egg by websites such as google.com
c. I would rewrite the code that is accessing this Easter Egg, most likely by fixing a simple syntax error.

8. 500

a. https://httpstat.us/500
b. There was a problem on the server's side
c. I'd try to use the website again, and use a different one if the problem persists.


For each of the questions below, write:

1. The website which generated the HTTP status code
2. A description of what the status code means
3. If an app you were writing encountered this status code, what would you do (if anything) to resolve any issues?


For reference, see:

https://en.wikipedia.org/wiki/List_of_HTTP_status_codes (Links to an external site.)
https://http.cat


# Part Two

API Scavenger Hunt!

For each of the questions below, identify a website and search query that will give you the appropriate JSON.  Paste the url and the json below.  Googling the category + API will generally take you to where you need.  Ex. https://lmgtfy.com/?q=cat+fact+api

1. A random cat fact

URL: https://catfact.ninja/fact
JSON: {
"fact": "Cats lap liquid from the underside of their tongue, not from the top.",
"length": 69
}

2. A list of 150 random users in English.

URL: https://api.randomuser.me/
JSON: {
"results": [
{
"gender": "male",
"name": {
"title": "mr",
"first": "matéo",
"last": "michel"
},
"location": {
"street": "5622 rue de l'abbé-gillet",
"city": "saint-denis",
"state": "haute-vienne",
"postcode": 85737,
"coordinates": {
"latitude": "-3.3048",
"longitude": "-14.9301"
},
"timezone": {
"offset": "-2:00",
"description": "Mid-Atlantic"
}
},
"email": "matéo.michel@example.com",
"login": {
"uuid": "ab588d6d-da67-4347-8fe1-e9d8e27e50b6",
"username": "whitebird930",
"password": "weed",
"salt": "ZOzEorCd",
"md5": "a294840b178e1ae8ff4e75c00e87e3ef",
"sha1": "11acb512d7b6acc5e67c52b9b126a4531252aad8",
"sha256": "2be30a1240e28da0105ea76bf1af5398d993d822f96156991cbd843ef3d57b46"
},
"dob": {
"date": "1975-03-24T05:10:55Z",
"age": 44
},
"registered": {
"date": "2016-01-16T22:02:42Z",
"age": 3
},
"phone": "05-14-93-06-33",
"cell": "06-53-56-27-95",
"id": {
"name": "INSEE",
"value": "1NNaN23458407 84"
},
"picture": {
"large": "https://randomuser.me/api/portraits/men/53.jpg",
"medium": "https://randomuser.me/api/portraits/med/men/53.jpg",
"thumbnail": "https://randomuser.me/api/portraits/thumb/men/53.jpg"
},
"nat": "FR"
}
],
"info": {
"seed": "cd960e913ad9cce0",
"results": 1,
"page": 1,
"version": "1.2"
}
}

3. The current stock price of Microsoft. (IEX API)

URL: https://cloud.iexapis.com/stable/stock/MSFT/quote
JSON: {
symbol: "MSFT",
companyName: "Microsoft Corp.",
primaryExchange: "NASDAQ",
calculationPrice: "close",
open: null,
openTime: null,
close: null,
closeTime: null,
high: null,
low: null,
latestPrice: 135.45,
latestSource: "Close",
latestTime: "August 26, 2019",
latestUpdate: 1566849600264,
latestVolume: null,
iexRealtimePrice: 135.435,
iexRealtimeSize: 100,
iexLastUpdated: 1566849594910,
delayedPrice: null,
delayedPriceTime: null,
extendedPrice: null,
extendedChange: null,
extendedChangePercent: null,
extendedPriceTime: null,
previousClose: 133.39,
previousVolume: null,
change: 2.06,
changePercent: 0.01544,
volume: null,
iexMarketPercent: 0.021865086875218123,
iexVolume: 440755,
avgTotalVolume: 26442955,
iexBidPrice: 0,
iexBidSize: 0,
iexAskPrice: 0,
iexAskSize: 0,
marketCap: 1034216284500,
peRatio: 26.51,
week52High: 141.67,
week52Low: 93.96,
ytdChange: 0.33456600000000003,
lastTradeTime: 1566849407072,
isUSMarketOpen: false
}

4. The 5 year history of Apple stock prices (IEX API)

URL: https://sandbox.iexapis.com/stable/stock/AAPL/chart/5y
JSON: [
{
date: "2014-08-25",
uClose: 102.16,
uOpen: 103.58,
uHigh: 105.77,
uLow: 104.77,
uVolume: 40963803,
close: 104.6,
open: 104.97,
high: 105.32,
low: 103.8,
volume: 41138115,
change: 0,
changePercent: 0,
label: "Aug 25, 14",
changeOverTime: 0
},
{
date: "2014-08-26",
uClose: 104.95,
uOpen: 102.97,
uHigh: 101.8,
uLow: 103.16,
uVolume: 33402484,
close: 104.05,
open: 106.03,
high: 106,
low: 103.17,
volume: 34360303,
change: -0.651,
changePercent: -0.6694,
label: "Aug 26, 14",
changeOverTime: -0.006669
}
]

5. All the Swift language repos on Github with Pursuit in their name


6. A list of all Pokemon

URL: https://pokeapi.co/api/v2/pokemon/
JSON: {
count: 964,
next: "https://pokeapi.co/api/v2/pokemon/?offset=20&limit=20",
previous: null,
results: [
{
name: "bulbasaur",
url: "https://pokeapi.co/api/v2/pokemon/1/"
},
{
name: "ivysaur",
url: "https://pokeapi.co/api/v2/pokemon/2/"
},
{
name: "venusaur",
url: "https://pokeapi.co/api/v2/pokemon/3/"
},
{
name: "charmander",
url: "https://pokeapi.co/api/v2/pokemon/4/"
},
{
name: "charmeleon",
url: "https://pokeapi.co/api/v2/pokemon/5/"
},
{
name: "charizard",
url: "https://pokeapi.co/api/v2/pokemon/6/"
},
{
name: "squirtle",
url: "https://pokeapi.co/api/v2/pokemon/7/"
},
{
name: "wartortle",
url: "https://pokeapi.co/api/v2/pokemon/8/"
},
{
name: "blastoise",
url: "https://pokeapi.co/api/v2/pokemon/9/"
}
]
}


7. A list of all items in Fortnite


8. A list of all Game of Thrones Episodes.


9. A list of all songs with "Love" in the title.

URL: https://itunes.apple.com/search?term=love
JSON: {
"resultCount":50,
"results": [
{"wrapperType":"track", "kind":"song", "artistId":42616562, "collectionId":715579496, "trackId":715581836, "artistName":"Nat \"King\" Cole", "collectionName":"Nat King Cole", "trackName":"L-O-V-E", "collectionCensoredName":"Nat King Cole", "trackCensoredName":"L-O-V-E", "artistViewUrl":"https://music.apple.com/us/artist/nat-king-cole/42616562?uo=4", "collectionViewUrl":"https://music.apple.com/us/album/l-o-v-e/715579496?i=715581836&uo=4", "trackViewUrl":"https://music.apple.com/us/album/l-o-v-e/715579496?i=715581836&uo=4", 
"previewUrl":"https://audio-ssl.itunes.apple.com/itunes-assets/AudioPreview71/v4/42/6a/a3/426aa324-78dd-8667-2869-dbfbb469e983/mzaf_5521623155491639858.plus.aac.p.m4a", "artworkUrl30":"https://is1-ssl.mzstatic.com/image/thumb/Music6/v4/50/b7/55/50b755d1-2721-ef0e-6898-c33d16be37f9/source/30x30bb.jpg", "artworkUrl60":"https://is1-ssl.mzstatic.com/image/thumb/Music6/v4/50/b7/55/50b755d1-2721-ef0e-6898-c33d16be37f9/source/60x60bb.jpg", "artworkUrl100":"https://is1-ssl.mzstatic.com/image/thumb/Music6/v4/50/b7/55/50b755d1-2721-ef0e-6898-c33d16be37f9/source/100x100bb.jpg", "collectionPrice":39.99, "trackPrice":1.29, "releaseDate":"1992-11-02T12:00:00Z", "collectionExplicitness":"notExplicit", "trackExplicitness":"notExplicit", "discCount":4, "discNumber":4, "trackCount":24, "trackNumber":24, "trackTimeMillis":152533, "country":"USA", "currency":"USD", "primaryGenreName":"Jazz", "isStreamable":true}

10. All information about Petyr Baelish from the Game of Thrones books


11. All the movies Leonardo Dicaprio has acted in

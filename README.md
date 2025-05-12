# cs546-lab-8--template-time-solved
**TO GET THIS SOLUTION VISIT:** [CS546 Lab 8 -Template Time Solved](https://www.ankitcodinghub.com/product/cs546-lab-8-template-time-solved/)


---

📩 **If you need this solution or have special requests:** **Email:** ankitcoding@gmail.com  
📱 **WhatsApp:** +1 419 877 7882  
📄 **Get a quote instantly using this form:** [Ask Homework Questions](https://www.ankitcodinghub.com/services/ask-homework-questions/)

*We deliver fast, professional, and affordable academic help.*

---

<h2>Description</h2>



<div class="kk-star-ratings kksr-auto kksr-align-center kksr-valign-top" data-payload="{&quot;align&quot;:&quot;center&quot;,&quot;id&quot;:&quot;91593&quot;,&quot;slug&quot;:&quot;default&quot;,&quot;valign&quot;:&quot;top&quot;,&quot;ignore&quot;:&quot;&quot;,&quot;reference&quot;:&quot;auto&quot;,&quot;class&quot;:&quot;&quot;,&quot;count&quot;:&quot;1&quot;,&quot;legendonly&quot;:&quot;&quot;,&quot;readonly&quot;:&quot;&quot;,&quot;score&quot;:&quot;5&quot;,&quot;starsonly&quot;:&quot;&quot;,&quot;best&quot;:&quot;5&quot;,&quot;gap&quot;:&quot;4&quot;,&quot;greet&quot;:&quot;Rate this product&quot;,&quot;legend&quot;:&quot;5\/5 - (1 vote)&quot;,&quot;size&quot;:&quot;24&quot;,&quot;title&quot;:&quot;CS546 Lab 8 -Template Time Solved&quot;,&quot;width&quot;:&quot;138&quot;,&quot;_legend&quot;:&quot;{score}\/{best} - ({count} {votes})&quot;,&quot;font_factor&quot;:&quot;1.25&quot;}">

<div class="kksr-stars">

<div class="kksr-stars-inactive">
            <div class="kksr-star" data-star="1" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="2" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="3" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="4" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="5" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
    </div>

<div class="kksr-stars-active" style="width: 138px;">
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
    </div>
</div>


<div class="kksr-legend" style="font-size: 19.2px;">
            5/5 - (1 vote)    </div>
    </div>
<div class="page" title="Page 1">
<div class="section">
<div class="section">
<div class="section">
<div class="layoutArea">
<div class="column">
CS-546 Lab 8 Template Time

For this lab, you will be using HTML, CSS, and Handlebars to make your first simple templated web application! You will be building a form that allows you to search through characters in the Marvel API.

You will not need to use a database for this lab.

You must use the async/await keywords (not Promises). You will also be using axios

(https://github.com/axios/axios) , which is a HTTP client for Node.js; you can install it with npm i axios . Marvel API

You will be using the Marvel API (https://developer.marvel.com) . You will need to register and sign up for an API key. You will not be able to make requests to the API without signing up and getting an API key

(https://developer.marvel.com/account) . You will use the Characters (https://gateway.marvel.com/v1/public/characters? ts=1592417963445&amp;apikey=a8f9ccf932bf29fd379ef00e11668673&amp;hash=f061194023791a1593a0ea861a27da67) listings

Please look at the data returned so you know the schema of the data and the objects it returns (the links to Characters above work but using my API key. DO NOT use my API key. Please register for your own. You will need to compose the URL with your API key, a ts (time stamp) and a hash.

You can use the following code to construct the URL. You can read more about AUTHORIZING AND SIGNING REQUESTS from the link below

https://developer.marvel.com/documentation/authorization (https://developer.marvel.com/documentation/authorization)

</div>
</div>
</div>
<div class="section">
<div class="layoutArea">
<div class="column">
<pre>const md5 = require('blueimp-md5');
const publickey = 'your_public_key(API KEY) from Marvel dev portal';
const privatekey = 'your private key from Marvel dev portal';
const ts = new Date().getTime();
const stringToHash = ts + privatekey + publickey;
const hash = md5(stringToHash);
</pre>
<pre>const baseUrl = 'https://gateway.marvel.com:443/v1/public/characters';
const url = baseUrl + '?ts=' + ts + '&amp;apikey=' + publickey + '&amp;hash=' + hash;
</pre>
</div>
</div>
</div>
<div class="layoutArea">
<div class="column">
<pre>https://gateway.marvel.com:443/v1/public/characters?nameStartsWith=SEARCH_TERM_HERE
</pre>
</div>
</div>
</div>
<div class="layoutArea">
<div class="column">
You will be using two endpoints of the Marvel API which is an API about Marvel for your Axios calls. The search character endpoint where you pass the search term as a query string parameter:

</div>
</div>
<div class="layoutArea">
<div class="column">
t i di id l h t i th d i t

</div>
</div>
<div class="layoutArea">
<div class="column">
https://sit.instructure.com/courses/50148/assignments/273388

</div>
<div class="column">
1/12

</div>
</div>
<div class="layoutArea">
<div class="column">
and then you’ll

</div>
</div>
</div>
</div>
<div class="page" title="Page 2">
<div class="section">
<div class="layoutArea">
<div class="column">
5/15/22, 11:35 AM Lab 8

</div>
</div>
<div class="section">
<div class="layoutArea">
<div class="column">
get an individual character using the endpoint

</div>
</div>
<div class="layoutArea">
<div class="column">
<pre>https://gateway.marvel.com:443/v1/public/characters/:id
</pre>
</div>
</div>
<div class="layoutArea">
<div class="column">
:id where :id is the ID of the character you are looking up.

You will use these two endpoints to make your axios.get calls depending on which route is called. You will be making three routes/pages in your application:

http://localhost:3000/ the main page of this application will provide a search form to start a search of characters for a keyword.

http://localhost:3000/search this page will make the axios call to the search endpoint and return up to 20 matching results that contain the provided request form param, searchTerm

http://localhost:3000/characters/{id} this page will show all the details of the character with the id matching the provided URL param, id

All other URLS should return a 404

</div>
</div>
<div class="layoutArea">
<div class="column">
<pre>## `GET http://localhost:3000/`
</pre>
</div>
</div>
<div class="layoutArea">
<div class="column">
&lt;title&gt;

<pre>/public/site.css
</pre>
</div>
</div>
<div class="layoutArea">
<div class="column">
input

<pre>POST http://localhost:3000/search
                       searchTerm
</pre>
</div>
<div class="column">
label

</div>
<div class="column">
<pre>/search
input
</pre>
</div>
<div class="column">
input

</div>
</div>
<div class="layoutArea">
<div class="column">
label

</div>
</div>
<div class="layoutArea">
<div class="column">
input

</div>
</div>
<div class="layoutArea">
<div class="column">
submit

</div>
</div>
<div class="layoutArea">
<div class="column">
searchTerm

spider

</div>
</div>
</div>
<div class="layoutArea">
<div class="column">
This page will respond with a valid HTML document. The title of the document should be “Character Finder”. You should have the title set as the element of the HTML document and as an h1 in your document.

Your page should reference a CSS file, ; this file should have at least 5 rulesets that apply to this page; these 5 rules can also apply to elements across all of your pages, or be unique to this page.

You should have a main element, and inside of the main element have a p element with a brief (2-3 sentence description) of what your website does.

Also inside the main element, you will have a form ; this form will POST to . This form will have an and a ; the should properly reference the same id as the . You should also have a with a type of that submits the form. The in your form where the user types the search term should have a name of .

This route will read the parameter and then make an axios call to the Marvel API endpoint searching for that keyword. For example, if the user typed in the input field, you would make the axios call to: https://gateway.marvel.com/v1/public/characters? nameStartsWith=SEARCH_TERM_HERE&amp;ts=TIME_STAMP_HERE&amp;apikey=API_KEY_HERE&amp;hash=HA

This route will respond with a valid HTML document with the results returned from the API. The title of

</div>
</div>
<div class="layoutArea">
<div class="column">
https://sit.instructure.com/courses/50148/assignments/273388 2/12

</div>
</div>
</div>
</div>
<div class="page" title="Page 3">
<div class="section">
<div class="layoutArea">
<div class="column">
5/15/22, 11:35 AM Lab 8

</div>
</div>
<div class="section">
<div class="section">
<div class="layoutArea">
<div class="column">
the document should be “Characters Found”. You should have the title set as the element of the HTML document and as an h1 in your document. In an h2 element, you will print the supplied

searchTerm .

Your page should reference a CSS file, /public/site.css ; this file should have at least 5 rulesets that

apply to this page; these 5 rules can also apply to elements on / , or be unique to this page.

You should have a main element, and inside of the main element have a ul tag that has a list of up to 20 characters matching the searchTerm found in the request body in the following format (after searching

under ). DO NOT SHOW MORE THAN 20 Characters.

</div>
</div>
</div>
<div class="section">
<div class="layoutArea">
<div class="column">
&lt;title&gt;

</div>
</div>
</div>
<div class="section">
<div class="layoutArea">
<div class="column">
&lt;ul&gt; &lt;li&gt;

<pre>        &lt;a href="/characters/1010727"&gt;Spider-dok&lt;/a&gt;
    &lt;/li&gt;
</pre>
<pre>    &lt;li&gt;
        &lt;a href="/characters/1009157"&gt;Spider-Girl (Anya Corazon)&lt;/a&gt;
</pre>
&lt;/li&gt; &lt;li&gt;

<pre>        &lt;a href="/Characters/1009609"&gt;Spider-Girl (May Parker)&lt;/a&gt;
    &lt;/li&gt;
</pre>
&lt;/ul&gt;

</div>
</div>
</div>
<div class="section">
<div class="layoutArea">
<div class="column">
You must also provide an a tag that links back to your / route with the text Make another search . If no matches are found, you will print the following HTML paragraph:

</div>
</div>
</div>
<div class="section">
<div class="layoutArea">
<div class="column">
<pre>&lt;p class="not-found"&gt;We're sorry, but no results were found for {searchTerm}.&lt;/p&gt;
</pre>
</div>
</div>
</div>
<div class="layoutArea">
<div class="column">
error

<pre>GET http://localhost:3000/characters/{id}
</pre>
</div>
</div>
<div class="layoutArea">
<div class="column">
&lt;title&gt;

</div>
</div>
<div class="layoutArea">
<div class="column">
<pre>/public/site.css
</pre>
</div>
</div>
<div class="layoutArea">
<div class="column">
<pre>thumbnail.path
</pre>
</div>
</div>
</div>
<div class="layoutArea">
<div class="column">
If the user does not input text into their form or enters just spaces into the input field, make sure to give a response status code of 400 on the page, and render an HTML page with a paragraph class called ; this paragraph should describe the error.

This route will query the Marvel API using the the id parameter in the URL (for example: https://gateway.marvel.com/v1/public/characters/1009609?

ts=TS_HERE&amp;apikey=API_KEY_HERE&amp;hash=HASH_HERE) and will respond with a valid HTML document with some of the character details. The title of the document should be the name of the character. You should have the title set as the element of the HTML document.

Your page should reference a CSS file, ; this file should have at least 5 rulesets that apply to this page; these 5 rules can also apply to elements on / , or be unique to this page.

You should have a main element, and inside of the main element, you will have a div tag that has an h1 with the character name , an img which the src is set to the value read from in the

data which is a URL to an image for the character, you will have a p element that contains the character https://sit.instructure.com/courses/50148/assignments/273388 3/12

</div>
</div>
</div>
</div>
<div class="page" title="Page 4">
<div class="layoutArea">
<div class="column">
5/15/22, 11:35 AM Lab 8

</div>
</div>
<div class="layoutArea">
<div class="column">
description , a h2 that’s content says “Comics” and a ul for the list of comics. You only need to display the comic name as the list items

Matching Character Data Returned from API (We will not be using all the fields, just the ones noted above):

<pre> {
   "code": 200,
   "status": "Ok",
   "copyright": "© 2021 MARVEL",
   "attributionText": "Data provided by Marvel. © 2021 MARVEL",
</pre>
</div>
</div>
<div class="layoutArea">
<div class="column">
<pre>  "attributionHTML": "&amp;lt;a href=\"http://marvel.com\"
Marvel. © 2021 MARVEL&amp;lt;/a&amp;gt;",
</pre>
<pre>  "etag": "284b3f7635608d1e18add4ff80c10902ef5959b4",
  "data": {
</pre>
<pre>    "offset": 0,
    "limit": 20,
    "total": 1,
    "count": 1,
    "results": [
</pre>
</div>
<div class="column">
(http://marvel.com/%22) ;&amp;gt;Data provided by

</div>
</div>
<div class="layoutArea">
<div class="column">
<pre>      {
        "id": 1009609,
        "name": "Spider-Girl (May Parker)",
        "description": "May \"Mayday\" Parker is the daughter of Spider-Man and Mary Jane Watson-Par
</pre>
<pre>ker. Born with all her fatherï¿1⁄2s powers-and the same silly sense of humor-sheï¿1⁄2s grown up to becom
e one of Earthï¿1⁄2s most trusted heroes and a fitting tribute to her proud papa.",
</pre>
</div>
</div>
<div class="layoutArea">
<div class="column">
<pre>        "modified": "2016-03-02T11:04:46-0500",
        "thumbnail": {
</pre>
“path”: “http://i.annihil.us/u/prod/marvel/i/mg/1/70/4c003adccbe4f prod/marvel/i/mg/1/70/4c003adccbe4f) “,

<pre>          "extension": "jpg"
        },
</pre>
“resourceURI”: “http://gateway.marvel.com/v1/public/characters/1009609 l.com/v1/public/characters/1009609) “,

</div>
<div class="column">
<pre>(http://i.annihil.us/u/
</pre>
<pre>  (http://gateway.marve
</pre>
</div>
</div>
<div class="layoutArea">
<div class="column">
<pre>        "comics": {
          "available": 196,
          "collectionURI": "http://gateway.marvel.com/v1/public/characters/1009609/comics
</pre>
ateway.marvel.com/v1/public/characters/1009609/comics) “, “items”: [

{

“resourceURI”: “http://gateway.marvel.com/v1/public/comics/5286 l.com/v1/public/comics/5286) “,

<pre>              "name": "Amazing Spider-Girl (2006)"
            },
</pre>
{

“resourceURI”: “http://gateway.marvel.com/v1/public/comics/5281 l.com/v1/public/comics/5281) “,

<pre>              "name": "Amazing Spider-Girl (2006) #1"
            },
</pre>
{

“resourceURI”: “http://gateway.marvel.com/v1/public/comics/5591 l.com/v1/public/comics/5591) “,

<pre>              "name": "Amazing Spider-Girl (2006) #2"
            },
</pre>
{

“resourceURI”: “http://gateway.marvel.com/v1/public/comics/5701 l.com/v1/public/comics/5701) “,

<pre>              "name": "Amazing Spider-Girl (2006) #3"
            },
</pre>
{

“resourceURI”: “http://gateway.marvel.com/v1/public/comics/5843 l.com/v1/public/comics/5843) “,

<pre>              "name": "Amazing Spider-Girl (2006) #4"
            },
</pre>
</div>
<div class="column">
(http://g

</div>
</div>
<div class="layoutArea">
<div class="column">
https://sit.instructure.com/courses/50148/assignments/273388

</div>
<div class="column">
4/12

</div>
</div>
<div class="layoutArea">
<div class="column">
<pre>(http://gateway.marve
</pre>
<pre>(http://gateway.marve
</pre>
<pre>(http://gateway.marve
</pre>
<pre>(http://gateway.marve
</pre>
<pre>(http://gateway.marve
</pre>
</div>
</div>
</div>
<div class="page" title="Page 5">
<div class="layoutArea">
<div class="column">
5/15/22, 11:35 AM }, Lab 8 {

“resourceURI”: “http://gateway.marvel.com/v1/public/comics/5997 l.com/v1/public/comics/5997) “,

<pre>                "name": "Amazing Spider-Girl (2006) #5"
              },
</pre>
{

“resourceURI”: “http://gateway.marvel.com/v1/public/comics/6130 l.com/v1/public/comics/6130) “,

<pre>                "name": "Amazing Spider-Girl (2006) #6"
              },
</pre>
{

“resourceURI”: “http://gateway.marvel.com/v1/public/comics/6270 l.com/v1/public/comics/6270) “,

<pre>                "name": "Amazing Spider-Girl (2006) #7"
              },
</pre>
{

“resourceURI”: “http://gateway.marvel.com/v1/public/comics/13478 l.com/v1/public/comics/13478) “,

<pre>                "name": "Amazing Spider-Girl (2006) #8"
              },
</pre>
{

“resourceURI”: “http://gateway.marvel.com/v1/public/comics/15856 l.com/v1/public/comics/15856) “,

<pre>                "name": "Amazing Spider-Girl (2006) #9"
              },
</pre>
{

“resourceURI”: “http://gateway.marvel.com/v1/public/comics/15966 l.com/v1/public/comics/15966) “,

<pre>                "name": "Amazing Spider-Girl (2006) #10"
              },
</pre>
{

“resourceURI”: “http://gateway.marvel.com/v1/public/comics/16151 l.com/v1/public/comics/16151) “,

<pre>                "name": "Amazing Spider-Girl (2006) #11"
              },
</pre>
{

“resourceURI”: “http://gateway.marvel.com/v1/public/comics/16522 l.com/v1/public/comics/16522) “,

<pre>                "name": "Amazing Spider-Girl (2006) #12"
              },
</pre>
{

“resourceURI”: “http://gateway.marvel.com/v1/public/comics/16523 l.com/v1/public/comics/16523) “,

<pre>                "name": "Amazing Spider-Girl (2006) #13"
              },
</pre>
{

“resourceURI”: “http://gateway.marvel.com/v1/public/comics/17249 l.com/v1/public/comics/17249) “,

<pre>                "name": "Amazing Spider-Girl (2006) #14"
              },
</pre>
{

“resourceURI”: “http://gateway.marvel.com/v1/public/comics/17385 l.com/v1/public/comics/17385) “,

<pre>                "name": "Amazing Spider-Girl (2006) #15"
              },
</pre>
{

l.com/v1/public/comics/17629) “,

“name”: “Amazing Spider-Girl (2006) #16”

}, {

“resourceURI”: “http://gateway.marvel.com/v1/public/comics/70668 l.com/v1/public/comics/70668) “,

<pre>                "name": "Amazing Spider-Girl (2006) #17"
              },
</pre>
{

</div>
<div class="column">
<pre>(http://gateway.marve
</pre>
<pre>(http://gateway.marve
</pre>
<pre>(http://gateway.marve
</pre>
<pre> (http://gateway.marve
</pre>
<pre> (http://gateway.marve
</pre>
<pre> (http://gateway.marve
</pre>
<pre> (http://gateway.marve
</pre>
<pre> (http://gateway.marve
</pre>
<pre> (http://gateway.marve
</pre>
<pre> (http://gateway.marve
</pre>
<pre> (http://gateway.marve
</pre>
<pre> (http://gateway.marve
</pre>
<pre> (http://gateway.marve
</pre>
</div>
</div>
<div class="layoutArea">
<div class="column">
<pre>"resourceURI": "http://gateway.marvel.com/v1/public/comics/17629
</pre>
</div>
</div>
<div class="layoutArea">
<div class="column">
https://sit.instructure.com/courses/50148/assignments/273388

</div>
<div class="column">
5/12

</div>
</div>
</div>
<div class="page" title="Page 6">
<div class="layoutArea">
<div class="column">
5/15/22, 11:35 AM { Lab 8

“resourceURI”: “http://gateway.marvel.com/v1/public/comics/20868 l.com/v1/public/comics/20868) “,

<pre>                "name": "Amazing Spider-Girl (2006) #18"
              },
</pre>
{

“resourceURI”: “http://gateway.marvel.com/v1/public/comics/21003 l.com/v1/public/comics/21003) “,

<pre>                "name": "Amazing Spider-Girl (2006) #19"
              }
</pre>
],

<pre>            "returned": 20
          },
</pre>
<pre>          "series": {
            "available": 37,
            "collectionURI": "http://gateway.marvel.com/v1/public/characters/1009609/series
</pre>
ateway.marvel.com/v1/public/characters/1009609/series) “, “items”: [

{

“resourceURI”: “http://gateway.marvel.com/v1/public/series/1126 l.com/v1/public/series/1126) “,

<pre>                "name": "Amazing Spider-Girl (2006 - 2009)"
              },
</pre>
{ l.com/v1/public/series/2234) “,

</div>
</div>
<div class="layoutArea">
<div class="column">
<pre>                                                                                         (http://gateway.marve
</pre>
PB (2007)”

},

{

“resourceURI”: “http://gateway.marvel.com/v1/public/series/3101 (http://gateway.marve

l.com/v1/public/series/3101) “,

“name”: “AMAZING SPIDER-GIRL VOL. 2: COMES THE CARNAGE! TPB (2007)”

</div>
</div>
<div class="layoutArea">
<div class="column">
<pre>"resourceURI": "http://gateway.marvel.com/v1/public/series/2234
"name": "AMAZING SPIDER-GIRL VOL. 1: WHATEVER HAPPENED TO THE DAUGHTER OF SPIDER-MAN T
</pre>
</div>
</div>
<div class="layoutArea">
<div class="column">
}, {

“resourceURI”: “http://gateway.marvel.com/v1/public/series/5376 l.com/v1/public/series/5376) “,

<pre>                "name": "Amazing Spider-Man Family (2008 - 2009)"
              },
</pre>
{

“resourceURI”: “http://gateway.marvel.com/v1/public/series/1143 l.com/v1/public/series/1143) “,

<pre>                "name": "Avengers Next (2006 - 2007)"
              },
</pre>
{

“resourceURI”: “http://gateway.marvel.com/v1/public/series/1995 l.com/v1/public/series/1995) “,

<pre>                "name": "Cable (1993 - 2002)"
              },
</pre>
{

“resourceURI”: “http://gateway.marvel.com/v1/public/series/5260 l.com/v1/public/series/5260) “,

<pre>                "name": "Counter X Vol. 1 (2008)"
              },
</pre>
{

“resourceURI”: “http://gateway.marvel.com/v1/public/series/19 om/v1/public/series/19) “,

<pre>                "name": "Daredevil Vol. II: Parts of a Hole (1999)"
</pre>
}, {

“resourceURI”: “http://gateway.marvel.com/v1/public/series/2119 l.com/v1/public/series/2119) “,

<pre>                "name": "Fantastic Five (1999 - 2000)"
              },
</pre>
{

l.com/v1/public/series/3281) “, https://sit.instructure.com/courses/50148/assignments/273388

</div>
<div class="column">
<pre>  (http://gateway.marve
</pre>
<pre>  (http://gateway.marve
</pre>
<pre>  (http://gateway.marve
</pre>
<pre>  (http://gateway.marve
</pre>
<pre>(http://gateway.marvel.c
</pre>
<pre>  (http://gateway.marve
</pre>
<pre>  (http://gateway.marve
</pre>
6/12

</div>
</div>
<div class="layoutArea">
<div class="column">
<pre>"resourceURI": "http://gateway.marvel.com/v1/public/series/3281
</pre>
</div>
</div>
<div class="layoutArea">
<div class="column">
<pre>(http://gateway.marve
</pre>
<pre>(http://gateway.marve
</pre>
</div>
</div>
<div class="layoutArea">
<div class="column">
<pre>(http://gateway.marve
</pre>
</div>
</div>
<div class="layoutArea">
<div class="column">
(http://g

</div>
</div>
</div>
<div class="page" title="Page 7">
<div class="layoutArea">
<div class="column">
5/15/22, 11:35 AM Lab 8

</div>
</div>
<div class="layoutArea">
<div class="column">
l.com/v1/public/series/3281) ,

“name”: “Fantastic Five: The Final Doom (2007)”

</div>
</div>
<div class="layoutArea">
<div class="column">
}, {

“resourceURI”: “http://gateway.marvel.com/v1/public/series/13881 l.com/v1/public/series/13881) “,

<pre>              "name": "Fear Itself: The Home Front (2010)"
            },
</pre>
{

“resourceURI”: “http://gateway.marvel.com/v1/public/series/2572 l.com/v1/public/series/2572) “,

<pre>              "name": "Iron Man (1998 - 2004)"
            },
</pre>
{

“resourceURI”: “http://gateway.marvel.com/v1/public/series/2031 l.com/v1/public/series/2031) “,

<pre>              "name": "J2 (1998 - 1999)"
            },
</pre>
{

“resourceURI”: “http://gateway.marvel.com/v1/public/series/923 com/v1/public/series/923) “,

<pre>              "name": "Last Hero Standing (2005)"
            },
</pre>
{

“resourceURI”: “http://gateway.marvel.com/v1/public/series/991 com/v1/public/series/991) “,

<pre>              "name": "Last Planet Standing (2006)"
            },
</pre>
{

“resourceURI”: “http://gateway.marvel.com/v1/public/series/322 com/v1/public/series/322) “,

<pre>              "name": "MARVEL AGE: SPIDER-GIRL VOL. 1: LEGACY DIGEST (2004)"
            },
</pre>
{

“resourceURI”: “http://gateway.marvel.com/v1/public/series/26878 l.com/v1/public/series/26878) “,

<pre>              "name": "Marvel's Greatest Creators: What If? - Spider-Girl (2019)"
            },
</pre>
{

“resourceURI”: “http://gateway.marvel.com/v1/public/series/2059 l.com/v1/public/series/2059) “,

<pre>              "name": "Paradise X (2002 - 2003)"
            },
</pre>
{

“resourceURI”: “http://gateway.marvel.com/v1/public/series/2431 l.com/v1/public/series/2431) “,

<pre>              "name": "Paradise X Vol. 1 (2007)"
            },
</pre>
{

“resourceURI”: “http://gateway.marvel.com/v1/public/series/2702 l.com/v1/public/series/2702) “,

<pre>              "name": "PARADISE X VOL. 2 TPB [NEW PRINTING] (2007)"
            }
</pre>
],

<pre>          "returned": 20
        },
</pre>
<pre>        "stories": {
          "available": 309,
</pre>
</div>
</div>
<div class="layoutArea">
<div class="column">
“collectionURI”: “http://gateway.marvel.com/v1/public/characters/1009609/stories (htt p://gateway.marvel.com/v1/public/characters/1009609/stories) “,

</div>
</div>
<div class="layoutArea">
<div class="column">
“items”: [ {

“resourceURI”: “http://gateway.marvel.com/v1/public/stories/791 l.com/v1/public/stories/791) “,

<pre>              "name": "Cover #791",
</pre>
<pre>              "type": "cover"
            },
</pre>
</div>
<div class="column">
<pre>(http://gateway.marve
</pre>
</div>
</div>
<div class="layoutArea">
<div class="column">
https://sit.instructure.com/courses/50148/assignments/273388

</div>
<div class="column">
7/12

</div>
</div>
<div class="layoutArea">
<div class="column">
<pre>  (http://gateway.marve
</pre>
<pre> (http://gateway.marve
</pre>
<pre> (http://gateway.marve
</pre>
<pre>(http://gateway.marvel.
</pre>
<pre>(http://gateway.marvel.
</pre>
<pre>(http://gateway.marvel.
</pre>
<pre>  (http://gateway.marve
</pre>
</div>
</div>
<div class="layoutArea">
<div class="column">
<pre>(http://gateway.marve
</pre>
<pre>(http://gateway.marve
</pre>
<pre>(http://gateway.marve
</pre>
</div>
</div>
</div>
<div class="page" title="Page 8">
<div class="layoutArea">
<div class="column">
5/15/22, 11:35 AM }, Lab 8 {

“resourceURI”: “http://gateway.marvel.com/v1/public/stories/792 l.com/v1/public/stories/792) “,

<pre>                "name": "Interior #792",
</pre>
<pre>                "type": "interiorStory"
              },
</pre>
{

“resourceURI”: “http://gateway.marvel.com/v1/public/stories/806 l.com/v1/public/stories/806) “,

<pre>                "name": "Cover #806",
</pre>
<pre>                "type": "cover"
              },
</pre>
{

“resourceURI”: “http://gateway.marvel.com/v1/public/stories/807 l.com/v1/public/stories/807) “,

<pre>                "name": "Interior #807",
</pre>
<pre>                "type": "interiorStory"
              },
</pre>
{

“resourceURI”: “http://gateway.marvel.com/v1/public/stories/808 l.com/v1/public/stories/808) “,

<pre>                "name": "Cover #808",
</pre>
<pre>                "type": "cover"
              },
</pre>
{

“resourceURI”: “http://gateway.marvel.com/v1/public/stories/809 l.com/v1/public/stories/809) “,

<pre>                "name": "Interior #809",
</pre>
<pre>                "type": "interiorStory"
              },
</pre>
{

“resourceURI”: “http://gateway.marvel.com/v1/public/stories/810 l.com/v1/public/stories/810) “,

<pre>                "name": "Cover #810",
</pre>
<pre>                "type": "cover"
              },
</pre>
{

“resourceURI”: “http://gateway.marvel.com/v1/public/stories/811 l.com/v1/public/stories/811) “,

<pre>                "name": "Interior #811",
</pre>
<pre>                "type": "interiorStory"
              },
</pre>
{

“resourceURI”: “http://gateway.marvel.com/v1/public/stories/812 l.com/v1/public/stories/812) “,

<pre>                "name": "Cover #812",
</pre>
<pre>                "type": "cover"
              },
</pre>
{

“resourceURI”: “http://gateway.marvel.com/v1/public/stories/813 l.com/v1/public/stories/813) “,

<pre>                "name": "Interior #813",
</pre>
<pre>                "type": "interiorStory"
              },
</pre>
{

“resourceURI”: “http://gateway.marvel.com/v1/public/stories/814 l.com/v1/public/stories/814) “,

<pre>                "name": "Cover #814",
</pre>
<pre>                "type": "cover"
              },
</pre>
{

“resourceURI”: “http://gateway.marvel.com/v1/public/stories/815 l.com/v1/public/stories/815) “,

<pre>                "name": "Interior #815",
</pre>
<pre>                "type": "interiorStory"
              },
</pre>
</div>
<div class="column">
<pre>(http://gateway.marve
</pre>
<pre>(http://gateway.marve
</pre>
<pre>(http://gateway.marve
</pre>
<pre>(http://gateway.marve
</pre>
<pre>(http://gateway.marve
</pre>
<pre>(http://gateway.marve
</pre>
<pre>(http://gateway.marve
</pre>
<pre>(http://gateway.marve
</pre>
<pre>(http://gateway.marve
</pre>
<pre>(http://gateway.marve
</pre>
<pre>(http://gateway.marve
</pre>
</div>
</div>
<div class="layoutArea">
<div class="column">
https://sit.instructure.com/courses/50148/assignments/273388

</div>
<div class="column">
8/12

</div>
</div>
</div>
<div class="page" title="Page 9">
<div class="layoutArea">
<div class="column">
5/15/22, 11:35 AM }, Lab 8

{

“resourceURI”: “http://gateway.marvel.com/v1/public/stories/816 l.com/v1/public/stories/816) “,

<pre>                "name": "Cover #816",
</pre>
<pre>                "type": "cover"
              },
</pre>
{

“resourceURI”: “http://gateway.marvel.com/v1/public/stories/817 l.com/v1/public/stories/817) “,

<pre>                "name": "Interior #817",
</pre>
<pre>                "type": "interiorStory"
              },
</pre>
{

“resourceURI”: “http://gateway.marvel.com/v1/public/stories/818 l.com/v1/public/stories/818) “,

<pre>                "name": "Cover #818",
</pre>
<pre>                "type": "cover"
              },
</pre>
{

“resourceURI”: “http://gateway.marvel.com/v1/public/stories/819 l.com/v1/public/stories/819) “,

<pre>                "name": "Interior #819",
</pre>
<pre>                "type": "interiorStory"
              },
</pre>
{

“resourceURI”: “http://gateway.marvel.com/v1/public/stories/820 l.com/v1/public/stories/820) “,

</div>
<div class="column">
<pre>(http://gateway.marve
</pre>
<pre>(http://gateway.marve
</pre>
<pre>(http://gateway.marve
</pre>
<pre>(http://gateway.marve
</pre>
<pre>(http://gateway.marve
</pre>
</div>
</div>
<div class="layoutArea">
<div class="column">
<pre>              "name": "\"THE PEOPLE PLAYED BY GAMES!\" Torn between her loyalties to Kaine and the B
lack Tarantula, Spider-Girl finally confronts Lady Oc",
</pre>
</div>
</div>
<div class="layoutArea">
<div class="column">
<pre>              "type": "cover"
            },
</pre>
{

“resourceURI”: “http://gateway.marvel.com/v1/public/stories/821 l.com/v1/public/stories/821) “,

</div>
<div class="column">
<pre>(http://gateway.marve
</pre>
</div>
</div>
<div class="layoutArea">
<div class="column">
<pre>              "name": "\"THE PEOPLE PLAYED BY GAMES!\" Torn between her loyalties to Kaine and the B
lack Tarantula, Spider-Girl finally confronts Lady Oc",
</pre>
</div>
</div>
<div class="layoutArea">
<div class="column">
<pre>              "type": "interiorStory"
            },
</pre>
{

“resourceURI”: “http://gateway.marvel.com/v1/public/stories/822 l.com/v1/public/stories/822) “,

</div>
<div class="column">
<pre>(http://gateway.marve
</pre>
</div>
</div>
<div class="layoutArea">
<div class="column">
<pre>              "name": "\"IF THIS BE MY DESTINY—!\" Spider-Girl learns the fate Norman Osborn planned
for his grandson when she finally uncovers the secre",
</pre>
</div>
</div>
<div class="layoutArea">
<div class="column">
<pre>              "type": "cover"
            },
</pre>
{

“resourceURI”: “http://gateway.marvel.com/v1/public/stories/823 l.com/v1/public/stories/823) “,

</div>
<div class="column">
<pre>(http://gateway.marve
</pre>
</div>
</div>
<div class="layoutArea">
<div class="column">
<pre>              "name": "\"IF THIS BE MY DESTINY—!\" Spider-Girl learns the fate Norman Osborn planned
for his grandson when she finally uncovers the secre",
</pre>
</div>
</div>
<div class="layoutArea">
<div class="column">
<pre>              "type": "interiorStory"
            }
</pre>
],

<pre>          "returned": 20
        },
</pre>
<pre>        "events": {
          "available": 1,
          "collectionURI": "http://gateway.marvel.com/v1/public/characters/1009609/events
</pre>
ateway.marvel.com/v1/public/characters/1009609/events) “, “items”: [

{

“resourceURI”: “http://gateway.marvel.com/v1/public/events/302 com/v1/public/events/302) “,

<pre>              "name": "Fear Itself"
            }
</pre>
],

<pre>          "returned": 1
</pre>
</div>
<div class="column">
(http://g

</div>
</div>
<div class="layoutArea">
<div class="column">
https://sit.instructure.com/courses/50148/assignments/273388 9/12

</div>
</div>
<div class="layoutArea">
<div class="column">
<pre>(http://gateway.marvel.
</pre>
</div>
</div>
</div>
<div class="page" title="Page 10">
<div class="layoutArea">
<div class="column">
5/15/22, 11:35 AM Lab 8

}, “urls”: [

</div>
</div>
<div class="layoutArea">
<div class="column">
<pre>{
  "type": "detail",
  "url": "http://marvel.com/characters/2171/spider-girl?utm_campaign=apiRef&amp;
</pre>
</div>
</div>
<div class="layoutArea">
<div class="column">
3″

},

{

“type”: “wiki”,

“url”: “http://marvel.com/universe/Spider-Girl_(MC2)?utm_campaign=apiRef&amp; (http://marve

l.com/universe/Spider-Girl_(MC2)?utm_campaign=apiRef&amp;) ;amp;utm_source=a8f9ccf932bf29fd379ef00e11668673” },

<pre>           {
             "type": "comiclink",
             "url": "http://marvel.com/comics/characters/1009609/spider-girl_may_parker?utm_campaign=
</pre>
apiRef&amp; (http://marvel.com/comics/characters/1009609/spider-girl_may_parker?utm_campaign=apiRef&amp;) ;amp;utm_ source=a8f9ccf932bf29fd379ef00e11668673″

} ]

} ]

} }

HTML Format Printed for the character. This will go into your main element:

<pre> &lt;div&gt;
   &lt;h1&gt;Spider-Girl (May Parker)&lt;/h1&gt;
   &lt;img alt= "Spider-Girl (May Parker)"src="http://i.annihil.us/u/prod/marvel/i/mg/1/70/4c003adccbe4f
</pre>
(http://i.annihil.us/u/prod/marvel/i/mg/1/70/4c003adccbe4f) “/&gt;

&lt;p&gt;May \”Mayday\” Parker is the daughter of Spider-Man and Mary Jane Watson-Parker. Born with all

<pre>  her fatherï¿1⁄2s powers-and the same silly sense of humor-sheï¿1⁄2s grown up to become one of Earthï¿1⁄2s
 most trusted heroes and a fitting tribute to her proud papa.&lt;/p&gt;
</pre>
<pre>   &lt;h2&gt;Comics&lt;/h2&gt;
   &lt;ul&gt;
</pre>
<pre>     &lt;li&gt;Amazing Spider-Girl (2006)&lt;/li&gt;
     &lt;li&gt;Amazing Spider-Girl (2006) #1&lt;/li&gt;
     &lt;li&gt;Amazing Spider-Girl (2006) #2&lt;/li&gt;
     &lt;li&gt;Amazing Spider-Girl (2006) #3&lt;/li&gt;
     &lt;li&gt;Amazing Spider-Girl (2006) #4&lt;/li&gt;
     &lt;li&gt;Amazing Spider-Girl (2006) #5&lt;/li&gt;
     &lt;li&gt;Amazing Spider-Girl (2006) #6&lt;/li&gt;
     &lt;li&gt;Amazing Spider-Girl (2006) #7&lt;/li&gt;
     &lt;li&gt;Amazing Spider-Girl (2006) #8&lt;/li&gt;
     &lt;li&gt;Amazing Spider-Girl (2006) #9&lt;/li&gt;
     &lt;li&gt;Amazing Spider-Girl (2006) #10&lt;/li&gt;
     &lt;li&gt;Amazing Spider-Girl (2006) #11&lt;/li&gt;
     &lt;li&gt;Amazing Spider-Girl (2006) #12&lt;/li&gt;
     &lt;li&gt;Amazing Spider-Girl (2006) #13&lt;/li&gt;
     &lt;li&gt;Amazing Spider-Girl (2006) #14&lt;/li&gt;
     &lt;li&gt;Amazing Spider-Girl (2006) #15&lt;/li&gt;
     &lt;li&gt;Amazing Spider-Girl (2006) #16&lt;/li&gt;
     &lt;li&gt;Amazing Spider-Girl (2006) #17&lt;/li&gt;
     &lt;li&gt;Amazing Spider-Girl (2006) #18&lt;/li&gt;
     &lt;li&gt;Amazing Spider-Girl (2006) #19&lt;/li&gt;
</pre>
&lt;/ul&gt; &lt;/div&gt;

If there is no character found for the given ID, make sure to give a response status code of 404 on the page, and render an HTML page with a paragraph class called error ; this paragraph should describe the error.

</div>
<div class="column">
(http://marv el.com/characters/2171/spider-girl?utm_campaign=apiRef&amp;) ;amp;utm_source=a8f9ccf932bf29fd379ef00e1166867

</div>
</div>
<div class="layoutArea">
<div class="column">
https://sit.instructure.com/courses/50148/assignments/273388

</div>
<div class="column">
10/12

</div>
</div>
</div>
<div class="page" title="Page 11">
<div class="section">
<div class="layoutArea">
<div class="column">
5/15/22, 11:35 AM

</div>
<div class="column">
Lab 8

</div>
</div>
<table>
<tbody>
<tr>
<td>
<div class="layoutArea">
<div class="column">
<pre>http://localhost:3000/public/site.css
</pre>
</div>
</div>
<div class="layoutArea">
<div class="column">
This file should have 5 rulesets that apply to the / route, and 5 rulesets that apply to all of your pages. Rulesets may be shared across both pages; for example, if you styled a p tag, it would count as 1 of the 5 for both pages.

You may include more than 5 rulesets if you so desire.

References and Packages

Basic CSS info can easily be referenced in the MDN CSS tutorial (https://developer.mozilla.org/en- US/docs/Web/Guide/CSS/Getting_started) .

Hints

You can use variables in your handlebars layout, that you pass to res.render. For example, in your layout you could have:

</div>
</div>
</td>
</tr>
<tr>
<td>
<div class="layoutArea">
<div class="column">
<pre>&lt;meta name="keywords" content="{{keywords}}" /&gt;
</pre>
</div>
</div>
</td>
</tr>
<tr>
<td>
<div class="layoutArea">
<div class="column">
And in your route:

</div>
</div>
</td>
</tr>
<tr>
<td>
<div class="layoutArea">
<div class="column">
<pre>res.render("someView", {keywords: "dogs coffee keto"});
</pre>
</div>
</div>
</td>
</tr>
<tr>
<td>
<div class="layoutArea">
<div class="column">
Which will render as:

</div>
</div>
</td>
</tr>
<tr>
<td>
<div class="layoutArea">
<div class="column">
<pre>&lt;meta name="keywords" content="dogs coffee keto" /&gt;
</pre>
</div>
</div>
</td>
</tr>
<tr>
<td>
<div class="layoutArea">
<div class="column">
Or, perhaps, the title tag.

Requirements

<ol>
<li>You must not submit your node_modules folder</li>
<li>You must remember to save your dependencies to your package.json folder</li>
<li>You must do basic error checking in each function</li>
<li>Check for arguments existing and of proper type.</li>
<li>Throw if anything is out of bounds (ie, trying to perform an incalculable math operation or accessing
data that does not exist)
</li>
<li>You MUST use async/await for all asynchronous operations.</li>
</ol>
7. You must remember to update your package.json file to set app.js as your starting script!

8. Your HTML must be valid (https://validator.w3.org/#validate_by_input) or you will lose points on the

assignment.

9. Your HTML must make semantical sense; usage of tags for the purpose of simply changing the style

</div>
</div>
</td>
</tr>
</tbody>
</table>
<div class="layoutArea">
<div class="column">
of elements (such as i b f t https://sit.instructure.com/courses/50148/assignments/273388

</div>
<div class="column">
t etc) will result in points being deducted; think in terms of 11/12

</div>
</div>
</div>
</div>
<div class="page" title="Page 12">
<div class="section">
<div class="layoutArea">
<div class="column">
5/15/22, 11:35 AM Lab 8

</div>
</div>
<div class="section">
<div class="section">
<div class="layoutArea">
<div class="column">
of elements (such as i , b , font , , etc) will result in points being deducted; think in terms of

content first, then style with your CSS.

10. You can be as creative as you’d like to fulfill front-end requirements; if an implementation is not

explicitly stated, however you go about it is fine (provided the HTML is valid and semantical). Design

is not a factor in this course.

11. All inputs must be properly labeled!

12. All previous requirements about the package.json author, start task, dependenices, etc. still apply

</div>
</div>
</div>
<div class="section">
<div class="layoutArea">
<div class="column">
center

</div>
</div>
</div>
</div>
<div class="layoutArea">
<div class="column">
https://sit.instructure.com/courses/50148/assignments/273388

</div>
<div class="column">
12/12

</div>
</div>
</div>
</div>

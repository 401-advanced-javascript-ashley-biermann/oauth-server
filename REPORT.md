# OAuth Comparative Analysis

## OAuth Provider - Yahoo!

### Research Conducted By: Ashley Biermann, Marlene Rinker (some time spent with Dave for a little bit)

### Overall Score and Comments
#### Score (Out of 10): 9
#### General Comments
- Yahoo requires the redirect uri to be an https, but we are only able to use http. We could not complete the create form without giving an https site. So, we proceeded as best we could.
- Marlene and I created a yahoo.js file and connected all the we could. Although we were not able to gain a client id and secret, we wrote the code as though we did. We are able to access the yahoo login page, but get an error that we don't have a client id. We considered this a success given that we were not able to get those pieces of information due to only using http.
- We also just experimented with the possiblity that one day our localhost could be https. We supplied the code for that as well as completed the create form and recieved client id and secret. Obviously we got errors that said it was not a secure connection, but it at least gave us the experience of creating an oauth app on Yahoo!'s site.
- Marlene also tried setting up a secure local host, but that did not prove successful in that the connection was still not secure. [Polygot](https://www.thepolyglotdeveloper.com/2018/11/create-self-signed-certificate-nodejs-macos/)
- Seems like the planning and prep time before actually starting to configure the oauth were the more difficult parts. We found others that also had limiting factors to getting started considering our short timeline. Google - needs a registered app. LinkedIn - needs an associated company. Apple - needs a certification set up. Amazon - ... I forget what the blocker was, but there was something.

#### Pros
* Great documentation
* Well-known

#### Cons
* For our lab, testing is difficult due to https requirement

### Ratings and Reviews
#### Documentation
- Easy to locate documentation
- Descriptive flow chart and corresponding steps, with sample resposes and success messages
- Errors and corresponding descriptions
- Troubleshooting sections

#### Systems Requirements
- Did not see anything in the documentation which covered this. We did find, however, as we tried to progress, that an `https` site was required for the redirect URI.

#### Ramp-Up Projections
- With a certificate for an `https` server, and this starter could, it would probably be reasonable to have something working within a day. But, it's hard to know for sure considering we got blocked and could not see into further possible issues.

#### Community Support and Adoption levels
- Did not see much about this. It feels like companies may be using other auth server options like Google.
- Is there an active community of developers supporting and growing it?
  - It's hard to say, but probably not. The [Yahoo Developer Network Feedback Forum](https://yahoo.uservoice.com/forums/309376-yahoo-mobile-developer-suite) on the oauth site leads to what we expected to be a helpful forum, but has very few responses to posts. It also links to the Verizon Media Dev Network, which was unexpected.

### Links and Resources
<!-- * [framework](http://xyz.com) -->
* [docs](https://developer.yahoo.com/oauth2/guide/)
* [examples/tutorials](https://developer.yahoo.com/oauth2/guide/flows_authcode/)

### Code Demos
<!-- * [live/running application](http://xyz.com) -->
* [code repository](https://github.com/401-advanced-javascript-ashley-biermann/oauth-server)

### Operating Instructions
* `npm start`
* Endpoint: `/`
  * Takes user to Yahoo! oauth link
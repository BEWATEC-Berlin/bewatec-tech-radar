# BEWATEC Tech-Radar

> This is a fork of https://github.com/thoughtworks/build-your-own-radar - so it makes sense to update from upstream from time to time.

## Contribution to it

> Everybody is more than welcome to keep an eye on it and to contribute to its completeness and correctness. 

Please clone locally, install dependencies and then go into dev mode, which allows you to see/check your changes immediately.

    git clone git@github.com:BEWATEC-Berlin/bewatec-tech-radar.git
    npm i
    npm run dev
    
Then open the URL http://127.0.0.1:8080/?documentId=/data.json in your browser.

To contribute to the radar, you can add/update/remove items from ./public/radar.json file.

Example of a data set:

    {
      "name": "some component/tool/...",
      "ring": "Trial",
      "quadrant": "Techniques",
      "isNew": "FALSE",
      "description": "<p>Whatever description you might add here. It can take HTML as well. <a href=\"www.google.de\">Google</a></p>"
    }

Once you are done with your changes, commit & push and create a pull request. Once accepted, the changes will automatically be deployed.

# How to use it?

## Quadrants

> Definition from ThoughtWorks.

  - ```Techniques``` These include elements of a software development process, such as experience design; and ways of structuring software, such as microservices.
  - ```Platforms``` - Things that we build software on top of such as mobile technologies like Android, virtual platforms like the JVM, or generic kinds of platforms like hybrid clouds.
  - ```Tools``` These can be components, such as databases, software development tools, such as version control systems; or more generic categories of tools, such as the notion of polyglot persistence.
  - ```languages-and-frameworks``` - Programming Languages and Frameworks. This was just languages but we rolled frameworks into here with the October 2012 Radar.

## Rings

> Definition from ThoughtWorks.

- The **Adopt** ring represents blips that we think you should seriously consider using. We don't say that you should use these for every project; any tool should only be used in an appropriate context. However, we do think that a blip in the Adopt ring represents something where there's no doubt that it's proven and mature for use.
- The **Trial** ring is for blips that we think are ready for use, but not as completely proven as those in the Adopt ring. So for most organizations, we think you should use these on a trial basis, to decide whether they should be part of your toolkit. Typically we've used trial blips in production, but we realize that readers are more cautious than us.
- The **Assess** ring are things to look at closely, but not necessarily trial yet - unless you think they would be a particularly good fit for you. Typically, blips in the Assess ring are things that we think are interesting and worth keeping an eye on.
- The **Hold** ring is for things that, even though they are accepted in the industry, we haven't had a good experience with. Therefore we are calling them out to warn you that you may run into trouble with them as well. Sometimes it means we think they're irredeemably flawed, or just being misused. We do place things in the Hold ring that we wish the industry wouldn't use.
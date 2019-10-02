# Sitegeist.Stencil.Roller
## Json API for headless Neos

**This is WIP, everything in here may change or turn out to be a bad idea at all.**

This packahe will expose the content of each document if the url is called using `.stencil.roller.json` suffix instead of `.html`;

The returned json:
```
{
   document: {
     identifier 
     nodeType
     properties: {
       // all properties of the node
     }  
     content: {
       // all children of type Content and ContentCollection recursively 
     } 
   }
   children: [{identifier, uri}, ..] // all children of type Document
}
```

### Authors & Sponsors

* Wilhelm Behncke - behncke@sitegeist.de
* Martin Ficzel - ficzel@sitegeist.de

*The development and the public-releases of this package is generously sponsored by our employer https://www.sitegeist.de.*

## Installation

Sitegeist.Stencil.Roller is available via packagist. Just run `composer require sitegeist/stencil-roller` to install it. We use semantic-versioning so every breaking change will increase the major-version number.

## Contribution

We will gladly accept contributions. Please send us pull requests.

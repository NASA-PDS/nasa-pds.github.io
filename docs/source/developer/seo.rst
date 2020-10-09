Search Engine Optimization
==========================

..  toctree::
    :maxdepth: 3

    seo

--------------

This brief guide will get you started with getting good results by
searches in major search engines. The goal of search engine optimization
(SEO) is to ensure your site gets found by planetary scientists who need
it. These tips and tricks will help you do that.

Search engines like Google or Bing catalog or “crawl” your site looking
for content, following hyperlinks, and gathering information about the
site to include in their indexes. When people type in search keywords,
the results use those indexes to give not just matching sites and pages,
but also ranking those pages against others for relevance. These ideas
will help you both match and get better ranking in the search results,
enabling you to reach more scientists eager for data.

Write for People
----------------

It used to be that search engines would just look for keywords. Now they
mimic more closely what human beings do on the web and imitate their
behavior. To that end, an easy thing to help with SEO is *write for
human beings*: don’t spam the same keyword over and over in text but
write naturally. Avoid using technical jargon about surfing the web
(don’t say “click here”, for example) but produce content as if you were
writing for a journal abstract or layperson article.

Make sure you always provide useful “alt text” for your images too. This
helps people with vision difficulties, sure, but also helps search
engines gain clues about the pictures on your site and how to include
them in search results.

Get a “Search Console”
----------------------

To make sure search engines are properly grabbing your site, register
for a free “search console” with search engine providers:

-  `Google Search
   Console <https://search.google.com/search-console/about>`__ (formerly
   “webmaster tools”) helps you make sure your site is being crawled.
-  `Bing Webmaster Tools <https://www.bing.com/toolbox/webmaster/>`__ is
   similar.

These tools will let you know if your site is being crawled at all, and
can warn you if parts of your site are giving errors. *They also will
help tell you if your site is mobile-friendly:* **more than half** of
all web browsing is done on smartphones and other mobile devices these
days. You want to make sure your reach these audiences!

Set up a Site Map
~~~~~~~~~~~~~~~~~

A site map is a standard in the XML format that tells search engines the
structure of your site. Some content management systems (CMSs) like
`WordPress <https://wordpress.org/>`__,
`Drupal <https://www.drupal.org/>`__, and `Plone <https://plone.org/>`__
automatically make a site map for you. Or you can make a ``sitemap.xml``
file yourself.

Smaller sites may not need a site map, but it doesn’t hurt to have one,
especially if it’s merely an option to turn on in your CMS.

You can `learn more about
sitemaps <https://support.google.com/webmasters/answer/156184?hl=en>`__
or try a `free sitemap generator tool <https://www.xml-sitemaps.com/>`__
online.

Set up a “robots.txt” File
~~~~~~~~~~~~~~~~~~~~~~~~~~

The ``robots.txt`` file is another web standard that gives hints to
search engines about what parts of your site to crawl—and especially
what parts *not* to crawl. There might be parts of your site you prefer
aren’t indexed and this is where you put this information. For example,
if you use a CMS, you don’t need the login page to be in search results,
so you might include ``/login`` in the ``robots.txt``.

You can also use it to tell search engines how fast or frequently to
crawl your site. If you’re hosting your node’s site on your kitchen
computer, you might want to limit just how fast Bing hammers your site
for all its pages especially when you’re looking up a recipe.

Modern CMSs like SquareSpace, Wix, and the others already mentioned will
usually make the ``robots.txt`` file for you. Or you can easily make
your own by `learning more about the
file <https://yoast.com/ultimate-guide-robots-txt/>`__. Your search
console will also tell you if it’s picking up your ``robots.txt``
properly.

Links
-----

One of the most important things you can do for SEO is make hyperlinks
to other sites with relevant content. That means PDS nodes should link
to other nodes and other websites. You don’t just have to link to
top-level sites either, but internal pages or other resources too. As
already stated above, make your link text useful phrases (i.e., don’t
hyperlink the word “here” in a phrase like “Click **here** to learn more
about NASA”; instead say “**More information about NASA** is available”
with multiple words hyperlinked.)

Even more important? Get other sites to *link to your site!* One of the
primary ways search engines determine your page rank (how high you
appear in search results) is how many other sites link to your site. You
might ask researchers using your data to include a link to your site.
You can also spread the word to your site through incoming links from
social media, like Facebook and Twitter postings. If a nearby university
does a feature on you, ask them to include a link to your site.

Data About Data
---------------

If the text of your web page is data, then information *about* that web
page is data about data, or *metadata*. Metadata is information not
usually visible (or only partially visible) to visitors of your site,
but is definitely there for crawlers to get.

Suppose a page on your site was
``https://my-pds-node.org/resources/gazetteer``. Some metadata about
that page would be:

-  *Title* = “Planetary Gazetteer”
-  *Description* = “An alphabetized guide of local planets and their
   satellites for use with planetary data lookups.”

Depending on your CMS, you might enter metadata like this just once for
your entire website. Others might let you customize metadata per-page.
If you’re making your web pages by hand, you’ll want to include metadata
in your HTML code; for example:

.. code:: html

   <html>
       <head>
           <title>Planetary Gazetteer</title>
           <meta name='description' content='An alphabetized guide of local planets and their satellites for use with planetary data lookups.'>
       </head>
       …
   </html>

Keywords used to be an important part of page metadata, but due to
“keyword stuffing” search engines began ignoring them (including `Google
in
2009 <https://webmasters.googleblog.com/2009/09/google-does-not-use-keywords-meta-tag.html>`__).
Other metadata that is still used is `Open Graph social
data <https://ogp.me/>`__, what `viewport to
provide <https://developer.mozilla.org/en-US/docs/Mozilla/Mobile/Viewport_meta_tag>`__
for mobile users, and so on. Your CMS may automate or provide tools to
help with this.

Get the Facts
-------------

Almost every question can be asked, “Relative to what?” Unless we have
some data to measure against, we can’t test if changes we make to our
site are having a positive or negative effects. That’s where *analytics*
comes in. Analytics is the `collection, measurement, and analysis of
website
use <https://www.usability.gov/what-and-why/web-analytics.html>`__. For
SEO, it means looking at what parts of our site are used and which are
under-used, what search keywords users find to discover our site, what
devices they surf on, their demographics, what referrals you’re getting
from other sites, and more.

With analytics, for example, you might find that many visitors to a
node’s site are searching for information about Saturn—which might be
wholly wrong if you happen to be the Planetary Plasma Interactions (PPI)
Node!

`Google Analytics <https://analytics.google.com/>`__ is the *de facto*
king of website analytics and is, thankfully, free. But `there are other
analytics
tools <https://contently.com/2016/08/02/the-top-10-free-content-analytics-tools/>`__
out there, and some site hosting platforms (like SquareSpace) have
analytics built-in.

Get some fresh coffee going because delving into analytics reports can
quickly become a new pastime! It can be fascinating to learn what search
terms people use to find your site (such as how frequently people
misspell “planetarry”) or what sites are linking to your site (you might
make some surprising discoveries and make some new connections when you
discover that a popular science blog is directing people your way).

Conclusion
----------

This is just the beginning of how to do some SEO of a node website.
There are numerous other resources out there including a free
`beginner’s guide to
SEO <https://contently.com/2016/08/02/the-top-10-free-content-analytics-tools/>`__
from Mozilla as well as paid SEO checkups and advice. In short, though,
writing naturally and for other humans, getting linked back and linking
to other sites, and registering with webmaster tools and analytics will
get you some great bang-for-the-buck.

May your search results be as highly ranked as your planetary data!

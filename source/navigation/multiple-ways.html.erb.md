---
title: Multiple Ways
status: editors-draft
order: 5
wcag_success_criteria:
  - 2.4.8
wcag_techniques:
  - G65
  - G161
  - G63
  - G127
---

For many users having different ways to access the content of a web site is beneficial. They may become confused by following long, involved navigation steps to access content. Others might arrive on a page deep in the hierarchy after clicking a link on the site or another sites and want to move up the hierarchy step by step to better understand the context.

## Breadcrumbs

Breadcrumbs help users to know where they are in the structure of a complete website. They are especially important on complex websites that have more than one or two levels of navigation.

Links in a breadcrumb navigation show a trail from the front page to the current page, with a link to every page on the way. Those links are usually separated by arrows. If images or icon fonts are used for the separators, they need to be used in an accessible way. The last item of the breadcrumb navigation should be the title of the current page, but not linked.

A breadcrumb navigation is usually positioned near the top of the page. As a navigational region, the `<nav>` element can be used, with an landmark role of `navigation` and a label “You are here:”.

{::nomarkdown}
<%= code_start() %>
{:/nomarkdown}

~~~ html
<nav class="breadcrumb" role="navigation" aria-label="You are here:">

    <a href="…">Home</a>

    &gt;

    <a href="…">SpaceBears</a>

    &gt;

    <span class="current">
        <span class="visuallyhidden">Current: </span>
        Cpt. Space 6 Plus
    </span>

</nav>
~~~

{::nomarkdown}
<%= code_end %>
{:/nomarkdown}

## Sitemap

A sitemap is a list of all pages of a website. It provides a good way to understand the structure of the website and can help users learn what the site contains and how content is organized. It is also an alternative to complex menu bars.

Simple sitemaps just show an outline view, while more complex sitemaps might also show complex relationship data as well. If the site map is large, it can make sense to show some levels of the hierarchy only when demanded from the user. A sitemap needs to stay updated when a page is added or deleted, should link to all sections of the site, and present the organization of the web site. See the [W3C <abbr title="Web Accessibility Initiative">WAI</abbr> sitemap](http://www.w3.org/WAI/sitemap.html) for an example.

## Search

A search option helps users to find content by entering certain keywords, which is often more efficient than going through the complete navigation looking for pages whose page title vaguely relates to the topic the user has in mind. Search functionality that spell-checks the entered terms and allows synonyms further increases its accessibility.

## Multiple ways to activate functions in applications

In addition to a menubar, similar functions can often be found in other sections of the application as well. For example functions can be activated by clicking icons, using the mouse context menu, or activating a keyboard shortcut.

# varnish 0.2.4

* Callout block titles have been improved: The underline height for titles have
  been fixed to not look wonky when titles have multiple lines (reported:
  @anenadic, #53; fixed @zkamvar, #55). Moreover, the text transformation will
  no longer affect `code` and `kbd` elements. 
* Heading element sizes have been recoded to use relative units. There was not 
  enough specification in the original CSS to properly distinguish between H3
  and H4 elements; moreover, on tablet and mobile devices, the H1 heading looked
  smallter than the H2 heading due to a copy/paste error. This has been fixed by
  using relative calcualtions (@zkamvar, #55)
* Sidebar navigation now says "Episodes" instead of "Expand" when collapsed so 
  that it is less confusing for folks. (suggested by @drmowinckels,
  https://github.com/carpentries/workbench/issues/16 (#47); fixed by @zkamvar, 
  #56)
* The collapsed sidebar label no longer reverts to saying "collapse" on a new
  page. 
* The hamburger menu for mobile devices now has a border so it's more clear
  that it is a menu (suggested by @drmowinckels,
  https://github.com/carpentries/workbench/issues/16 (#47); fixed by @zkamvar, 
  #57)


# varnish 0.2.3

* Add support for displaying anchor links (requested @fiveop, 
  https://github.com/carpentries/sandpaper/issues/285 and @anenadic, 
  https://github.com/carpentries/workbench/issues/28; added: #54 by @zkamvar)

# varnish 0.2.2

* Formatting of list elements in the solutions and instructor notes now follows
  the same formatting as the rest of the content (reported: #51 by @tobyhodges, 
  fixed: #52 by @zkamvar)

# varnish 0.2.1

* The sidebar navigation in mobile and tablet views now includes all the 
  information that was included in the navigation bar for the desktop mode. 
  (reported: https://github.com/carpentries/workbench/issues/16#issuecomment-1165307355 by @Athanasiamo and #49, fixed: #50 by @zkamvar)

# varnish 0.2.0

* The sidebar state (expanded or collapsed) will now persist during navigation
  to another page in the same window/tab. Opening the site in a new window/tab
  will reset the sidebar state to expanded. (reported: #43 by @anenadic, fixed
  #46, @zkamvar). This fix uses the `sessionStorage` API. 

# varnish 0.1.16

* CHAPTERS has been temporarily renamed to EPISODES to reduce cognative load
  between the webpage and the source folders

# varnish 0.1.15

* The search field has been disabled to avoid confusion. We have not yet enabled
  search as this requires further testing. Disabling the search field means that
  it is now more clear that search is not yet available.
  (#44 by @zkamvar)

# varnish 0.1.14

* indicators for lesson development stage (pre-alpha, alpha, beta) have been 
  added as `<abbr>` elements with a link to the appropriate section in the CDH
  and `title` elements that describe the purpose of the stage. Visually hidden
  text follows the `<abbr>` element for users who can not perceive the lesson
  visually (#39 by @zkamvar, reviewed by @tobyhodges).
* FIX: .lesson-title and .lesson-title-md are now inline-block elements

# varnish 0.1.13

* An alert for the workbench beta phase is implemented if the lesson has
  `workbench-beta: true` in the `config.yaml`.

# varnish 0.1.12

* dropdown navigation no longer is hidden by the sidebar on XXL screens;
  z-index of `nav.bottom-nav` set to 3.
  (reported: #35 by @brownsarahm, fixed: #36 by @zkamvar)

# varnish 0.1.11
 
* blockquotes are now more clearly delineated from the rest of the content
  (reported: #27 by @fiveop, fixed: #31 by @zkamvar)

# varnish 0.1.10

* lab and incubator logos are now available.

# varnish 0.1.9

* Fix missing pegboard version tag

# varnish 0.1.8

* custom workbench engines are now properly linked in the footer via the 
  `sandpaper_cfg` `pegboard_cfg`, and `varnish_cfg` variables.
* code of conduct link now points to the `CODE_OF_CONDUCT.md` file so authors
  can update or modify their own code of conduct (NOTE: all Carpentries lessons
  MUST have a code of conduct that links to the Carpentries Code of Conduct as
  well as the reporting guidelines.

# varnish 0.1.7

* compile the changes from 0.1.6

# varnish 0.1.6

* Tables now scroll on overflow

# varnish 0.1.5

* The index page now has specific sections for schedule and setup that link to
  the `#schedule` and `#setup` anchors. This partially addresses 
  https://github.com/carpentries/sandpaper/issues/260

# varnish 0.1.4

* Removed " logo" suffix from the logo elements, as it is redundant
  https://webaim.org/techniques/alttext/#logos

# varnish 0.1.3

* Add small version of the carpentries logo

# varnish 0.1.2

* Add matmo analytics in the footer (@fmichonneau, #17)

# varnish 0.1.1

* Add LICENSE file clarifying MIT licensing

# varnish 0.1.0

* Breaking change; moving from the carpentries/styles theme to the new theme
  developed in 2021. Variables and layouts have changed significantly, so this
  package gains a significant update.

# varnish 0.0.0.9008

* instructor block placeholder added

# varnish 0.0.0.9007

* update css to use em and not px
* align logo with navbar
* add testing phase notification to navbar

# varnish 0.0.0.9006

* First tracked version of varnish
* updated links to engines in the footer

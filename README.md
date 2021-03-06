MagicSuggest v1.2
--------------------------

Check out full documentation and examples here: http://nicolasbize.github.com/magicsuggest/

Milestone change log:

v1.2.6 BugFix
=============
- (fix) suggestions were not appearing when maxSuggestions was set to 10. (credits to zerekw - https://github.com/zerekw and plasmaxy - https://github.com/plasmaxy)

v1.2.5 BugFix and added a couple of missing functions
=====================================================
- (fix) the clear function was broken (credits to travishaagen - https://github.com/travishaagen)
- (fea) the component's config can now be setup entirely from the DOM container element.
- (fea) added a silent mode to selection changing methods in order to know if it was user-triggered or not. (credits to travishaagen - https://github.com/travishaagen)
- (fea) added a setData(object) method to fill the combo after it has been rendered (credits to travishaagen - https://github.com/travishaagen)

v1.2.4 BugFix and toggle collapse/expand on click option
========================================================
- (fix) ajax query was sent twice when the user was typing faster than the typeDelay (credits to arvenom - https://github.com/arvenom)
- (fix) highlighting the search results was also highlighting html tags when using custom rendering (credits to pstuart2 - https://github.com/pstuart2)
- (fea) added cfg(strictSuggest) so that user can choose how the suggestions will be made
- (fea) added cfg(toggleOnClick) so that the user can expand/close the combo by clicking on it (credits to psulek - https://github.com/psulek)

v1.2.3 BugFix and selection rendering
=====================================
- (fix) empty suggestion text was wrongly triggered when performing initial ajax call (credits to curtgrimes - https://github.com/curtgrimes)
- (fea) added cfg(selectionRenderer) (credits to pstuart2 - https://github.com/pstuart2)

v1.2.2 IE compatibility, rendering options
==========================================
- (fix) empty text class was not triggered properly (credits to jods4 - https://github.com/jods4)
- (fix) IE8 compatibility (credits to Airborn22 - https://github.com/Airborn22)
- (fea) MagicSuggest can now be rendered from a select dom component. (credits to Yogu - https://github.com/Yogu)
- (fea) on blur now automatically adds the typed text to the selection if free entries are allowed (credits to Airborn22 - https://github.com/Airborn22)
- (fea) new public method empty() which will clear the user text.

v1.2.1 Bugfixing
================
- (fix) make sure combo is filled prior to triggering load event
- (fea) renamed some events for better readability

v1.2.0 Standardization on jQuery plugins (Minor Tagged Milestone - Mar. 4th 2013)
=================================================================================
- (fix) fixed disabled behaviour when one could still edit the emptyText
- (fix) collapse method would throw an error
- (cfg) typeDelay: Amount (in ms) between keyboard registers (credits to jayesbee - https://github.com/jayesbee)
- (fea) standardized on jQuery plugin (credits to jayesbee - https://github.com/jayesbee)
- (fea) added documentation examples
- (cfg) name: name used for magicsuggest as a form element (credits to iambibhas - https://github.com/iambibhas)
- (fix) start up rendering when value rendered as text
- (cfg) dataParams: additional parameters for ajax request (credits to jayesbee - https://github.com/jayesbee)
- (fix) other rendering issues with inner text

v1.1.0 Various enhancements and bug fixing (Minor Tagged Milestone - Feb. 19th 2013)
====================================================================================
- (fea) close cross style now blends in a bit more
- (fea) escape now collapses the combo (without loosing focus)
- (fix) can't enter entries made out of space
- (cfg) noSuggestionText: text displayed when there are no suggestions from given data
- (cfg) minCharsRenderer: allows to customize message when not enough characters are entered to trigger a search
- (cfg) maxEntryRenderer: allows to customize message when too many characters have been entered
- (cfg) maxEntryLength: amount of characters to limit user input
- (cfg) style: custom style applied to the main container
- (cfg) infoMsgCls: custom class to apply to the helper
- (fea) new helper message on upper right to inform on the component status
- (cfg) id: allows to give the component a custom ID
- (cfg) inputCfg : allows additional parameters passed out to the INPUT tag. Enables usage of AngularJS's custom tags for ex.
- (cfg) renderer : allows custom rendering within the combo.
- (cfg) groupBy : allows grouping within the combo box listing.
- (fix) blur event now registers correctly when selecting an element from the combo
- (fix) flicker in IE when hovering trigger
- (cfg) strictSuggest : set how suggestions will be proposed
- (fix) maxResults is now correctly interpreted
- (fix) maxSelection is now correctly interpreted
- (cfg) method : set the ajax method, default to 'POST'
- (fea) ajax request can now interpret multiple results from server base.
- (fix) bug where the blur event would be triggered when clicking upon the page
- (cfg) required : triggers invalid / valid events when not filled
- (fea) validation through isValid() method

v1.0. initial component release
===============================
- choose to allow free entries or not
- keyboard management
- theme ability
- static and dynamic data processing
- positionning
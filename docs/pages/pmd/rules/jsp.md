---
title: Java Server Pages Rules
tags: [rule_references, jsp]
summary: Index of all built-in rules available for Java Server Pages
language_name: Java Server Pages
permalink: pmd_rules_jsp.html
folder: pmd/rules
---
## Best Practices

{% include callout.html content="Rules which enforce generally accepted best practices." %}

*   [DontNestJsfInJstlIteration](pmd_rules_jsp_bestpractices.html#dontnestjsfinjstliteration): Do not nest JSF component custom actions inside a custom action that iterates over its body.
*   [NoClassAttribute](pmd_rules_jsp_bestpractices.html#noclassattribute): Do not use an attribute called 'class'. Use "styleclass" for CSS styles.
*   [NoHtmlComments](pmd_rules_jsp_bestpractices.html#nohtmlcomments): In a production system, HTML comments increase the payloadbetween the application server to the c...
*   [NoJspForward](pmd_rules_jsp_bestpractices.html#nojspforward): Do not do a forward from within a JSP file.

## Code Style

{% include callout.html content="Rules which enforce a specific coding style." %}

*   [DuplicateJspImports](pmd_rules_jsp_codestyle.html#duplicatejspimports): Avoid duplicate import statements inside JSP's.

## Design

{% include callout.html content="Rules that help you discover design issues." %}

*   [NoInlineScript](pmd_rules_jsp_design.html#noinlinescript): Avoid inlining HTML script content.  Consider externalizing the HTML script using the 'src' attri...
*   [NoInlineStyleInformation](pmd_rules_jsp_design.html#noinlinestyleinformation): Style information should be put in CSS files, not in JSPs. Therefore, don't use <B> or <FONT>tags...
*   [NoLongScripts](pmd_rules_jsp_design.html#nolongscripts): Scripts should be part of Tag Libraries, rather than part of JSP pages.
*   [NoScriptlets](pmd_rules_jsp_design.html#noscriptlets): Scriptlets should be factored into Tag Libraries or JSP declarations, rather than being part of J...

## Error Prone

{% include callout.html content="Rules to detect constructs that are either broken, extremely confusing or prone to runtime errors." %}

*   [JspEncoding](pmd_rules_jsp_errorprone.html#jspencoding): A missing 'meta' tag or page directive will trigger this rule, as well as a non-UTF-8 charset.

## Security

{% include callout.html content="Rules that flag potential security flaws." %}

*   [IframeMissingSrcAttribute](pmd_rules_jsp_security.html#iframemissingsrcattribute): IFrames which are missing a src element can cause security information popups in IE if you are ac...
*   [NoUnsanitizedJSPExpression](pmd_rules_jsp_security.html#nounsanitizedjspexpression): Avoid using expressions without escaping / sanitizing. This could lead to cross site scripting - ...

## Additional rulesets

*   Basic JSP (`rulesets/jsp/basic.xml`):

    <span style="border-radius: 0.25em; color: #fff; padding: 0.2em 0.6em 0.3em; display: inline; background-color: #d9534f; font-size: 75%;">Deprecated</span>  This ruleset is for backwards compatibility.

    It contains the following rules:

    [DuplicateJspImports](pmd_rules_jsp_codestyle.html#duplicatejspimports), [IframeMissingSrcAttribute](pmd_rules_jsp_security.html#iframemissingsrcattribute), [JspEncoding](pmd_rules_jsp_errorprone.html#jspencoding), [NoClassAttribute](pmd_rules_jsp_bestpractices.html#noclassattribute), [NoHtmlComments](pmd_rules_jsp_bestpractices.html#nohtmlcomments), [NoInlineScript](pmd_rules_jsp_design.html#noinlinescript), [NoInlineStyleInformation](pmd_rules_jsp_design.html#noinlinestyleinformation), [NoJspForward](pmd_rules_jsp_bestpractices.html#nojspforward), [NoLongScripts](pmd_rules_jsp_design.html#nolongscripts), [NoScriptlets](pmd_rules_jsp_design.html#noscriptlets), [NoUnsanitizedJSPExpression](pmd_rules_jsp_security.html#nounsanitizedjspexpression)



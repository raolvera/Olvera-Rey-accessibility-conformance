# Accessibility Audit Notes

Project: Community Tech Day Accessibility Practice Page
Author: Rey Olvera
Course: GIT 515 Advanced Web Coding
Module: 5 Accessibility Conformance
Due: September 27, 2026


## 1. Run one tool-based check and record what it finds

I ran the starter page through the W3C HTML validator, the W3C CSS validator, and the browser DevTools. I checked it against WCAG 2.1 A and AA. The first pass found four problems in seven places. The submit button had no name. Two form fields had no label. Three links failed the color contrast rule. One heading level was skipped. I ran the checks again after my fixes, and the button, the labels, and the focus outline no longer showed up.

## 2. Test keyboard navigation and visible focus manually

I put the mouse aside and moved through the page using only the Tab key. The focus order was fine and matched how you read the page. The problem was that I could not see where I was. The stylesheet had turned off the focus outline on links, buttons, and inputs and did not add anything back. I removed that rule and gave focus a clear outline. I also added a skip to main content link at the top so a keyboard user does not have to tab through the whole header. Now I can see the outline on each link, button, and input as I move.

## 3. Check landmarks, headings, links, buttons, and image alternatives

The landmarks were mostly there. The starter had a header, a nav, and a main, but the nav had no name. The links were a clearer problem. All three cards used the word More, even though each one went to a different place. That is no help in a screen reader link list. The button was the worst part. The submit button had nothing inside it, so I gave it the word Register. I also checked the card images. They are decorative and sit next to a heading that already names each card.

The two that mattered most were the empty button and the link and label naming. I carried those into the issue list below.

## 4. Test zoom and reflow at 200 percent or a narrow responsive condition

I set the browser to 200 percent zoom at about 1280 pixels. Then I dragged the window in to a phone width. Both times the page made me scroll sideways. The cause was that the header and the main area were locked to a fixed width near 980 pixels.

## 5. Issues found, with evidence, impact, priority, fix, and retest

The assignment asks for at least five issues found and at least three fixed. I found five issues and fixed the three High ones. I marked an issue High when it blocks a task, Medium when it is a serious barrier, and Low for smaller problems.

Issue 1, the empty submit button, was High. The button had no text, so a screen reader read it as just button. It sits on the main action of the page, so I put it first. I added the word Register inside the button. On the retest it now reads as Register button and passes.

Issue 2, the unlabeled form fields, was also High. The Name field used a plain span that only looked like a label. The Email field had a label that was never linked to its input. Clicking the text did nothing, and a screen reader never named the field. I made both into real labels with a for attribute pointing at each input id, and I marked them required. Now each field announces its name and required state.

Issue 3, the missing focus outline, was High. The stylesheet had set outline none on links, buttons, and inputs with no replacement. A keyboard user could not tell where they were, so it blocked keyboard use. I gave focus a clear outline again. Now every interactive element shows a ring as I tab onto it.

Issue 4, the broken layout at zoom, was Medium. I found it but have not fixed it yet. The header and main area are pinned near 980 pixels, so zooming in or viewing on a phone forces sideways scrolling. The planned fix is to use a flexible max-width, let the header wrap, and stack everything into one column.

Issue 5, the low contrast links, was Medium. I found it but have not fixed it yet. The card links are a light gray on white at about 4.29 to 1, which is under the 4.5 to 1 that normal text needs. That makes them hard for low vision readers to see. The planned fix is to move them to the darker brand maroon at about 8.88 to 1.

## 6. Retest the fixed items and document what changed

I retested the three fixes I made. The empty submit button now reads as Register button. The two form fields announce their name and required state. The focus outline now shows on every interactive element as I tab through. The two Medium issues, the zoom layout and the low contrast links, are still open and would be my next fixes.

## 7. One issue the checker tools caught and one issue only manual testing revealed

The empty submit button is the one the tools caught. The scan flagged it right away, because a button with no text and no name is an easy pattern for a checker to find. The missing focus outline is the one the tools missed. The scan called the page clean, so on paper nothing was wrong. But as soon as I started tabbing with the keyboard, I could see there was no way to tell where focus was. A checker cannot feel that. It only showed up because I moved through the page the way a keyboard user would.

# Accessibility-Interview-Questions-Answers
| No. | Questions & Answers                                                                                                                                                  |
| --- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| 1   | What is WAI-ARIA? <br/><br/> WAI-ARIA is a technology that can be used to add extra information about the structure and function of a page. This can be especially helpful for users with disabilities who are using assistive technologies.
| 2   | What is the WCAG? <br/><br/> The Web Content Accessibility Guidelines (WCAG) are a set of standards for making web content accessible to people with disabilities. The WCAG is developed by the World Wide Web Consortium (W3C), an international standards body. There are three levels in WCAG 2.1, Level A (the lowest level), Level AA, and Level AAA (the highest level). These are usually pronounced as ‘single A’, ‘double A’, and ‘triple A’. Most organisations set their standards at level AA because it is both achievable and meaningful, without being too disruptive to the design and development process of a website. 
| 3   | Level A guidelines that should get followed by organizations: <br/><br/> 1) Alt text for images is compulsory.<br/> 2) For pre-recorded audio-only or video-only media, provide a descriptive transcript to make it understandable.<br/> 3) Headings should be nested appropriately.<br/> 4) ARIA labels should be there at specific places to make them recognizable.<br/> 5) Don’t use div and span; rather, use real elements like links and buttons.<br/> 6) Content should be in a meaningful way.<br/> 7)Content shouldn’t be based only on shape, size, color, sound, or other sensory characteristics.<br/> 8) If using color for words, background, or links, provide its information in the text.<br/> 9) Avoid including audio or video in content that plays automatically.<br/> 10) Make sure the user can navigate the content using only keyboard as well.<br/> 11) There should be pause, stop, hide for moving elements like, videos and animations.<br/> 12) Never use such an element that blink more than three times in 1 second.<br/> 13) Don’t give irrelevant links.Give descriptive labels in form fields or use ARIA-described by to include help text in forms.
| 4   | Level AA guidelines that should get followed by organizations:<br/><br/> 1) Captions are needed for live audio and video. Also, videos should include narration for better reach.Device orientation should not be the problem for content. 2) It should be available in both horizontal and vertical forms on all devices. 3) The color contrast of text is 4.5:1, for text and image 3:1, and the text size should be a minimum of 16px. 4) Content on hover or focus should appear adequately and should not overlap other content.The website should contain any of these - a table of contents, sitemap, or a list of related pages. 5) Headings and labels of each page should be unique. 6) Keyboard focus should be highly visible, and visible elements should have focused all the time if using the keyboard. 7) The same component on a web page should appear in a consistent order.To convey a status message, use ARIA live regions or ARIA alert to make it understandable for screen readers. 8) Web forms should have accurate labels and navigation.
| 5   | How do I know if my website is compliant with WCAG standards? <br/><br/> Your website should adhere to the four principles of WCAG in order to be considered compliant. The four principles are outlined in the acronym “POUR” which stands for Perceivable, Operable, Understandable, and Robust. You can also use an accessibility checker like UserWay’s Accessibility Scanner to determine your WCAG conformance. More recently, many countries (or states and provinces) across the globe have adopted WCAG as the basis for their accessibility standards and regulations – including regulations such as the <strong>EU Web Accessibility Directive</strong>, <strong>the AODA in Canada</strong>, and of course, <strong>Section 508 Compliance</strong> in the United States.
| 6   | What is the difference between alt text and longdesc? <br/><br/> Alt text and longdesc are two ways of adding descriptions to images on the web. <br/> 1) Alt text is a brief description that is displayed in place of an image if the image cannot be loaded. alt text is primarily used to describe the visual content. <br/> 2) Longdesc is a longer description that can be accessed by clicking on a link or icon. longdesc can be used to provide information about the function of an image.
| 7   | What is the difference between a screen reader and a text-to-speech program? <br/><br/> A screen-reader is a software program that assists blind or visually-impaired users by reading aloud the text that is displayed on the computer screen. A text-to-speech program, on the other hand, is a software application that converts written text into spoken words. <br/> Both screen-readers and text-to-speech programs can be used to improve accessibility for individuals with vision impairments, but they differ in terms of functionality and features. <br/> Screen-readers are specifically designed to work with computer applications and websites, while text-to-speech programs can be used to convert any written text into speech. Screen-readers also typically offer a wider range of features than text-to-speech programs, such as the ability to navigate websites and control the cursor without using a mouse.
| 8   | What is the most popular screen reader? <br/><br/> the most popular one is JAWS (Job Access With Speech). Other options are NVDA (NonVisual Desktop Access), Window-Eyes, VoiceOver (built into MacOS) and Orca (built into Linux).
| 9   | What is the most popular screen reader? <br/><br/> text-to-speech (TTS) programs have become increasingly popular. TTS programs allow users to input text and convert it into speech. Natural Reader is the clear choice for the most popular TTS program.
| 10   | We want to hide content from the screen readers how you will do? <br/><br/> There are a few ways through which we can hide the content from the screen readers: 1) Hiding images: aria-hidden="true" and role="presentation" 2) To completely hide from the screen readers use display:none
| 11   | Is infinite scrolling accessibility friendly? <br/><br/> No, it is not accessible at all. We should have the data loading only on-demand such as on click of the button
| 12   | What is the shortcut key to activate and deactivate the screenreader (Voice over) on Mac <br/><br/> fn + cmmd + F5 : To toggle the Voiceover
| 13   | What is ARIA? While creating a Tab module how you will decide the ARIA tags? <br/><br/> ARIA stands for Accessible Rich Internet Application. ARIA is useful for screenreader users. It won't create any difference visually. There are many tags, states, and properties missing from the HTML tags. Also, there are many custom modules we make such as carousels, pagination, etc which are not defined in the HTML. These are impossible for screenreader users to understand. ARIA provides information about such modules by defining the roles, properties, and states for screenreaders. In short, ARIA is the bridge between missing information in HTML and screenreaders.
| 14   | For accessibility should we use em or rem? <br/><br/> For accessibility, it is preferred to use rem for the margin/padding and em for the font-size. One more way we can do here is: `html{ font-size: 100%; }`
| 15   | What is VPAT? <br/><br/> It is a non-official document used by the products to share information about their product's accessibility level.
| 16   | For screen readers users on an e-commerce website after an item got added to the cart how you will notify them? <br/><br/> ARIA-live can be used here. We can decide between "polite" or "assertive". polite will wait for the user to finish the action and wait for the screenreader to finish the work. However, assertive will announce immediately. Disrupting the flow.
| 17   | What is the difference between legend, caption, and label elements? <br/><br/> Legends are used to describe the information in the charts or help in mapping the information with the graphical content. <br/> Captions are used to identify or describe an entire chart or graphical content. These care kind of - titles. <br/> label is used with form inputs to give information about what that field is about.
| 18   | Name an ARIA attribute that requires either a child/parent relationship or a pairing role. <br/><br/> 1) tablist and tab 2) radiogroup and radio




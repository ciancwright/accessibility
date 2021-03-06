# Accessibility audit report

| Client      | NHSx                               |
| ----------- | ---------------------------------- |
| Service     | Covid-19 app                       |
| Standard    | WCAG 2.1 AA                        |
| Audit by    | Cian Wright                        |
| Start       | Thursday 30 July 2020              |
| This report | Thursday 30 July 2020              |
| Contact     | cian.c.wright@accenture.com        |

## Build details

- iOS build Version 3.0
- Android build #

## Executive summary

An accessibility report for the NHSx COVID-19 mobile application. The application was assessed against WCAG 2 Mobile Accessibility Guidelines. Full details below in [Appendix: Reference].

### Classification of Issues

The following scoring system was used to indicate the status of the app with regards to each WCAG 2.0 AA Guidelines

| Status                      | Description                                                                                                                                                                                             |
| --------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| :white_check_mark: Pass                  | The app meets the requirement                                                                                                                                                   |
| :heavy_exclamation_mark: Risk | The app meets the requirement but is at risk
| :red_circle: Fail                  | The app fails to meet the requirement                                                              |
| :white_circle: (N/A) Not Applicable       | No relevant content was found    

The following violations need fixing in order to comply.

| Platform | Status | Success Criteria                             |
| -------- | ----- | ----------------------------------------------- |
| iOS      | 🔴 | 1.1.1 Non-text Content                         |
| iOS      | 🔴 | 1.3.1 Info and Relationships                         |
| iOS      | 🔴 | 1.4.4 Resize Text           |
| iOS      | 🔴 | 2.3.1 Three Flashes or Below Threshold                         |
| iOS      | 🔴 | 2.4.6 Headings and Labels                         |
| iOS      | 🔴 | 3.2.3 Consistent Navigation                         |
| iOS      | 🔴 | 3.2.4 Consistent Identification
| iOS      | 🔴 | 4.1.2 Name, Role, Value                         |

The following pass the requirements but are at risk of failing.

| Platform | Status | Success Criteria                             |
| -------- | ----- | ----------------------------------------------- |
| iOS      | :heavy_exclamation_mark: | 2.4.3 Focus Order                                   |
| iOS      | :heavy_exclamation_mark: | 2.4.4 Link Purpose (In Context)                         |
| iOS      | :heavy_exclamation_mark: | Guideline 3.2 Predictable                         |
| iOS      | :heavy_exclamation_mark: | 3.3.1 Error Identification                         |

## Technical Notes

#### 1.1.1 Non-text Content
First element on each startup, home and about screen cause screen reader to state "Repeat <number> counts" on first load.
  
Scroll on "About" screen incorrectly reads page wrong, skipping page 2 and therefore repeating "page 1/3 of 3" twice.

Home screen pulsing image has large touch area before reporting symptoms. However, once symptoms are reported, the touch area disappears and each individual element (heading, date, number, and days to go text) are individual elements but are incorrectly marked for the screen reader, instead repeating "The app is scanning your position" for each.

#### 1.3.1 Info and Relationships
"More info", "Read latest advice" and "How the app works" links identifying as a button. Review symptoms date selector identifies as a button.

#### 1.4.4 Resize Text
Text set to largest causes header on Venue Check In screen to be too close to the Close button causing potential issues for screen readers.

#### 2.3.1 Three Flashes or Below Threshold
Observed to meet the reqirement of not exceeding three flashes per animation cycle, however the animation repeats therefore exceeding this threshold. Notably, the rate of pulsing changes depending on the condition.

When navigating away from the app (following a link) and back, the animation pulsing is no longer a smooth transition, and instead flashes and staggers.

Also note that these pulses continue when text is on the screen (such as the "You need to isolate" message). This causes potential issues to users with reading impairment or with visual sensitivity due to the constantly changing colours behind the text. In monochrome mode, it is unclear as to what is being conveyed.

#### 2.4.3 Focus Order
"Cancel" button on Select symptoms screen focus blocks scroll from working unless another element is selected.

#### 2.4.4 Link Purpose (In Context) 
The purpose of the "How the app works" link is clearly identifiable, however this heading is also present in the "About" section accessed from the Navigation Bar. This information should be grouped together, ideally with the link presented at the bottom of this section within the About screen in the same way other links are presented on this screen. 

#### 2.4.6 Headings and Labels
The information within "Exposure Notification" on the second start up screen refers to both Google and Apple unnecessarily.

Info text on Book a free test screen displays "virology_book_a_test_explanation"

#### Guideline 3.2 Predictable
On the start up screen, important elements appear at the bottom of the screen including requirements before activating the app, privacy and terms of use links and actionable buttons. These follow a logical presentation order as per 1.3.2, but may present difficulties to users unfamiliar with scroll functionality. Consider placing these buttons outside of the scroll and these important links above the privacy and data information.

#### 3.2.3 Consistent Navigation
Menu and link options are not consistent throughout the app. From the home screen, the options direct the user to a camera, a self-report and redirect to a link otuside of the app. From the 'About' option on the Navigation Bar, these links redirecting to a website outside of the app are presented differently (in the standard underline and colour change).

Scrolling on "Select Symptoms" with screen reader active is blocked while the "Cancel" button is in focus. This is the default focus for this screen, and scrolling cannot be performed unless another element is selected.

#### 3.2.4 Consistent Identification
The "More info" option from the top of the home screen, "Read latest advice" and "How the app works" buttons navigate to a website outside of the app, but are not consistently presented with links in the "About" screen.

#### 3.3.1 Error Identification
Able to select symptoms and still navigate to "I don't have any of these symptoms".

#### 4.1.2 Name, Role, Value
"More info", "Read latest advice" and "How the app works" links identifying as a button. Review symptoms date selector identifies as a button.

## Accessibility Test Results
### 1 Perceivable
Information and user interface components must be presentable to users in ways they can perceive.

#### 1.1 Text Alternatives
Provide text alternatives for any non-text content so that it can be changed into other forms people need, such as large print, braille, speech, symbols or simpler language.

| iOS   | Android | Level | Success Criterion                                                                  |
| ----- | ------- | ----- | ---------------------------------------------------------------------------------- |
| 🔴 |    | A     | [1.1.1 Non-text Content](https://www.w3.org/WAI/WCAG21/quickref/#non-text-content) |

#### 1.2 Time-based Media
Provide alternatives for time-based media.

| iOS     | Android | Level | Success Criterion                                                                                                                                        |
| ------- | ------- | ----- | -------------------------------------------------------------------------------------------------------------------------------------------------------- |
| ⚪️ | ⚪️ | A     | [1.2.1 Audio-only and Video-only (Prerecorded)](https://www.w3.org/WAI/WCAG21/quickref/#audio-only-and-video-only-prerecorded)                           |
| ⚪️ | ⚪️ | A     | [1.2.2 Captions (Prerecorded)](https://www.w3.org/WAI/WCAG21/quickref/#captions-prerecorded)                                                             |
| ⚪️ | ⚪️ | A     | [1.2.3 Audio Description or Media Alternative (Prerecorded)](https://www.w3.org/WAI/WCAG21/quickref/#audio-description-or-media-alternative-prerecorded) |
| ⚪️ | ⚪️ | AA    | [1.2.4 Captions (Live)](https://www.w3.org/WAI/WCAG21/quickref/#captions-live)                                                                           |
| ⚪️ | ⚪️ | AA    | [1.2.5 Audio Description (Prerecorded)](https://www.w3.org/WAI/WCAG21/quickref/#audio-description-prerecorded)                                           |

#### 1.3 Adaptable
Create content that can be presented in different ways (for example simpler layout) without losing information or structure.

| iOS     | Android | Level | Success Criterion                                                                                             |
| ------- | ------- | ----- | ------------------------------------------------------------------------------------------------------------- |
| 🔴 |  | A     | [1.3.1 Info and Relationships](https://www.w3.org/WAI/WCAG21/quickref/#info-and-relationships)                |
| :white_check_mark: |  | A     | [1.3.2 Meaningful Sequence](https://www.w3.org/WAI/WCAG21/quickref/#meaningful-sequence)                      |
| :white_check_mark: |  | A     | [1.3.3 Sensory Characteristics](https://www.w3.org/WAI/WCAG21/quickref/#sensory-characteristics)              |
| :white_check_mark: |  | AA    | [1.3.4 Orientation](https://www.w3.org/WAI/WCAG21/quickref/#orientation) (Added in 2.1)                       |
| ⚪️ | ⚪️ | AA    | [1.3.5 Identify Input Purpose](https://www.w3.org/WAI/WCAG21/quickref/#identify-input-purpose) (Added in 2.1) |

#### 1.4 Distinguishable
Make it easier for users to see and hear content including separating foreground from background.

| iOS     | Android | Level | Success Criterion                                                                                                    |
| ------- | ------- | ----- | -------------------------------------------------------------------------------------------------------------------- |
| 🔴 |  | A     | [1.4.1 Use of Color](https://www.w3.org/WAI/WCAG21/quickref/#use-of-color)                                           |
| ⚪️ | ⚪️ | A     | [1.4.2 Audio Control](https://www.w3.org/WAI/WCAG21/quickref/#audio-control)                                         |
| :white_check_mark: | :white_check_mark: | AA    | [1.4.3 Contrast (Minimum)](https://www.w3.org/WAI/WCAG21/quickref/#contrast-minimum)                                 |
| :heavy_exclamation_mark: | :white_check_mark: | AA    | [1.4.4 Resize text](https://www.w3.org/WAI/WCAG21/quickref/#resize-text)                                             |
| :white_check_mark: | :white_check_mark: | AA    | [1.4.5 Images of Text](https://www.w3.org/WAI/WCAG21/quickref/#images-of-text)                                       |
| ⚪️ | ⚪️ | AA    | [1.4.10 Reflow](https://www.w3.org/WAI/WCAG21/quickref/#reflow) (Added in 2.1)                                       |
| ⚪️ | ⚪️ | AA    | [1.4.11 Non-text Contrast](https://www.w3.org/WAI/WCAG21/quickref/#non-text-contrast) (Added in 2.1)                 |
| ⚪️ | ⚪️ | AA    | [1.4.12 Text Spacing](https://www.w3.org/WAI/WCAG21/quickref/#text-spacing) (Added in 2.1)                           |
| ⚪️ | ⚪️ | AA    | [1.4.13 Content on Hover or Focus](https://www.w3.org/WAI/WCAG21/quickref/#content-on-hover-or-focus) (Added in 2.1) |

### 2 Operable
User interface components and navigation must be operable.

#### 2.1 Keyboard Accessible
Make all functionality available from a keyboard.

| iOS     | Android | Level | Success Criterion                                                                                               |
| ------- | ------- | ----- | --------------------------------------------------------------------------------------------------------------- |
| :white_check_mark: | :white_check_mark: | A     | [2.1.1 Keyboard](https://www.w3.org/WAI/WCAG21/quickref/#keyboard)                                              |
| :white_check_mark: | :white_check_mark: | A     | [2.1.2 No Keyboard Trap](https://www.w3.org/WAI/WCAG21/quickref/#no-keyboard-trap)                              |
| ⚪️ | ⚪️ | A     | [2.1.4 Character Key Shortcuts](https://www.w3.org/WAI/WCAG21/quickref/#character-key-shortcuts) (Added in 2.1) |

#### 2.2 Enough Time
Provide users enough time to read and use content.

| iOS     | Android | Level | Success Criterion                                                                    |
| ------- | ------- | ----- | ------------------------------------------------------------------------------------ |
| ⚪️ | ⚪️ | A     | [2.2.1 Timing Adjustable](https://www.w3.org/WAI/WCAG21/quickref/#timing-adjustable) |
| ⚪️ | ⚪️ | A     | [2.2.2 Pause, Stop, Hide](https://www.w3.org/WAI/WCAG21/quickref/#pause-stop-hide)   |

### 2.3 Seizures and Physical Reactions
Do not design content in a way that is known to cause seizures or physical reactions.

| iOS     | Android | Level | Success Criterion                                                                                                       |
| ------- | ------- | ----- | ----------------------------------------------------------------------------------------------------------------------- |
| 🔴 | ⚪️ | A     | [2.3.1 Three Flashes or Below Threshold](https://www.w3.org/WAI/WCAG21/quickref/#three-flashes-or-below-threshold)      |

### 2.4 Navigable
Provide ways to help users navigate, find content, and determine where they are.

| iOS     | Android | Level | Success Criterion                                                                                  |
| ------- | ------- | ----- | -------------------------------------------------------------------------------------------------- |
| ⚪️ | ⚪️ | A     | [2.4.1 Bypass Blocks](https://www.w3.org/WAI/WCAG21/quickref/#bypass-blocks)                       |
| :white_check_mark: |  | A     | [2.4.2 Page Titled](https://www.w3.org/WAI/WCAG21/quickref/#page-titled)                           |
| :heavy_exclamation_mark: |  | A     | [2.4.3 Focus Order](https://www.w3.org/WAI/WCAG21/quickref/#focus-order)                           |
| :heavy_exclamation_mark: | | A     | [2.4.4 Link Purpose (In Context)](https://www.w3.org/WAI/WCAG21/quickref/#link-purpose-in-context) |
| ⚪️ | ⚪️ | AA    | [2.4.5 Multiple Ways](https://www.w3.org/WAI/WCAG21/quickref/#multiple-ways)                       |
| 🔴 |  | AA    | [2.4.6 Headings and Labels](https://www.w3.org/WAI/WCAG21/quickref/#headings-and-labels)           |
| :white_check_mark: |  | AA    | [2.4.7 Focus Visible](https://www.w3.org/WAI/WCAG21/quickref/#focus-visible)                       |

#### 2.5 Input Modalities
Make it easier for users to operate functionality through various inputs beyond keyboard.

| iOS     | Android | Level | Success Criterion                                                                                                       |
| ------- | ------- | ----- | ----------------------------------------------------------------------------------------------------------------------- |
| :white_check_mark: |  | A     | [2.5.1 Pointer Gestures](https://www.w3.org/WAI/WCAG21/quickref/#pointer-gestures) (Added in 2.1)                       |
| :white_check_mark: |  | A     | [2.5.2 Pointer Cancellation](https://www.w3.org/WAI/WCAG21/quickref/#pointer-cancellation) (Added in 2.1)               |
| ⚪️ |  | A     | [2.5.3 Label in Name](https://www.w3.org/WAI/WCAG21/quickref/#label-in-name) (Added in 2.1)                             |
| ⚪️ |  | A     | [2.5.4 Motion Actuation](https://www.w3.org/WAI/WCAG21/quickref/#motion-actuation) (Added in 2.1)                       |

### 3 Understandable
Information and the operation of user interface must be understandable.

#### 3.1 Readable
Make text content readable and understandable.

| iOS   | Android | Level | Success Criterion                                                                    |
| ----- | ------- | ----- | ------------------------------------------------------------------------------------ |
| :white_check_mark: |  | A     | [3.1.1 Language of Page](https://www.w3.org/WAI/WCAG21/quickref/#language-of-page)   |
| :white_check_mark: |  | AA    | [3.1.2 Language of Parts](https://www.w3.org/WAI/WCAG21/quickref/#language-of-parts) |

#### 3.2 Predictable
Make screens appear and operate in predictable ways.

| iOS   | Android | Level | Success Criterion                                                                                    |
| ----- | ------- | ----- | ---------------------------------------------------------------------------------------------------- |
| :white_check_mark: |  | A     | [3.2.1 On Focus](https://www.w3.org/WAI/WCAG21/quickref/#on-focus)                                   |
| :white_check_mark: |  | A     | [3.2.2 On Input](https://www.w3.org/WAI/WCAG21/quickref/#on-input)                                   |
| 🔴 |  | AA    | [3.2.3 Consistent Navigation](https://www.w3.org/WAI/WCAG21/quickref/#consistent-navigation)         |
| 🔴 |  | AA    | [3.2.4 Consistent Identification](https://www.w3.org/WAI/WCAG21/quickref/#consistent-identification) |

#### 3.3 Input Assistance
Help users avoid and correct mistakes.

| iOS     | Android | Level | Success Criterion                                                                                                                |
| ------- | ------- | ----- | -------------------------------------------------------------------------------------------------------------------------------- |
| :heavy_exclamation_mark: | | A     | [3.3.1 Error Identification](https://www.w3.org/WAI/WCAG21/quickref/#error-identification)                                       |
| :white_check_mark: |  | A     | [3.3.2 Labels or Instructions](https://www.w3.org/WAI/WCAG21/quickref/#labels-or-instructions)                                   |
| :white_check_mark: |  | AA    | [3.3.3 Error Suggestion](https://www.w3.org/WAI/WCAG21/quickref/#error-suggestion)                                               |
| :white_check_mark: |  | AA    | [3.3.4 Error Prevention (Legal, Financial, Data)](https://www.w3.org/WAI/WCAG21/quickref/#error-prevention-legal-financial-data) |

### Robust
Content must be robust enough that it can be interpreted by by a wide variety of user agents, including assistive technologies.

#### 4.1 Compatible 
Maximize compatibility with current and future user agents, including assistive technologies.

| iOS     | Android | Level | Success Criterion                                                                               |
| ------- | ------- | ----- | ----------------------------------------------------------------------------------------------- |
| ⚪️ | ⚪️ | A     | [4.1.1 Parsing](https://www.w3.org/WAI/WCAG21/quickref/#parsing)                                |
| 🔴 | | A     | [4.1.2 Name, Role, Value](https://www.w3.org/WAI/WCAG21/quickref/#name-role-value)              |
| :white_check_mark: | :white_check_mark: | AA    | [4.1.3 Status Messages](https://www.w3.org/WAI/WCAG21/quickref/#status-messages) (Added in 2.1) |

## Appendix: Reference

- [Mobile Accessibility: How WCAG 2.0 and other W3C/WAI Guidelines Appply to Mobile](https://www.w3.org/TR/mobile-accessibility-mapping)
- [WCAG 2.0 Techniques that Apply to Mobile](https://www.w3.org/WAI/GL/mobile-a11y-tf/MobileTechniques)
- [How to Meet WCAG (Quick Reference)](https://www.w3.org/WAI/WCAG21/quickref)

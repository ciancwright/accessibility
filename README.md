# Accessibility audit report

| Client      | NHSx                               |
| ----------- | ---------------------------------- |
| Service     | Covid-19 app                       |
| Standard    | WCAG 2.1 AA                        |
| Audit by    | Cian Wright                        |
| Start       | Saturday 4 April 2020              |
| This report | Saturday 9 May 2020                |
| Contact     | cian.c.wright@accenture.com        |

## Build details

- iOS build 1.0.2 (356)
- Android build 1.0.0.224 (9a01637)

## Executive summary

An accessibility audit for the NHSx CoLocate mobile application was carried out by Phil Sherry. The application was assessed against the Web Content Accessibility Guidelines (WCAG) 2.1, **which it failed to meet to level AA**. Full details below in [Appendix I: Web Content Accessibility Guidelines (WCAG) 2.1](#appendix-i-web-content-accessibility-guidelines-wcag-21).

The following violations need fixing in order to comply to a AA standard.

| Platform | Level | Success Criterion                               |
| -------- | ----- | ----------------------------------------------- |
| iOS      | 🔴 (H) | 1.1.1 Non-text Content                          |
| Android  | 🔴 (H) | 1.3.1 Info and Relationships                    |
| Both     | 🔴 (H) | 1.4.1 Use of Color                              |
| Both     | 🟠 (M) | 1.4.3 Contrast (Minimum)                        |
| Both     | 🟠 (M) | 1.4.4 Resize text                               |
| Both     | 🔴 (H) | 2.4.2 Page Titled                               |
| iOS      | 🔴 (H) | 2.4.4 Link Purpose (In Context)                 |
| Both     | 🟠 (M) | 2.4.6 Headings and Labels                       |
| Both     | 🟠 (M) | 2.4.7 Focus Visible                             |
| iOS      | 🔴 (H) | 2.4.9 Link Purpose (Link Only)                  |
| Both     | 🔴 (H) | 3.3.1 Error Identification                      |
| Both     | 🟠 (M) | 3.3.4 Error Prevention (Legal, Financial, Data) |
| Android  | 🔴 (H) | 4.1.2 Name, Role, Value                         |

The following violations need fixing in order to comply to a AAA standard.

| Platform | Level | Success Criterion            |
| -------- | ----- | ---------------------------- |
| Both     | 🟣 (L) | 2.4.10 Section Headings      |
| iOS      | 🟣 (L) | 2.5.5 Target Size            |
| Both     | 🟣 (L) | 3.3.6 Error Prevention (All) |

## Technical summary

### 1.1.1 Non-text Content



### 1.3.1 Info and Relationships



### 1.4.1 Use of Color



### 1.4.3 Contrast (Minimum)


### 1.4.4 Resize text


### 2.4.2 Page Titled



#### Headings throughout the app



### 2.4.4 Link Purpose (In Context)


### 2.4.6 Headings and Labels



### 2.4.7 Focus Visible


### 2.4.9 Link Purpose (Link Only)


### 2.4.10 Section Headings


### 2.5.5 Target Size


### 3.3.1 Error Identification


### 3.3.4 Error Prevention (Legal, Financial, Data)


### 3.3.6 Error Prevention (All)


### 4.1.2 Name, Role, Value



## Audit results

### Test the service with various native settings on an Android device

- **Screen:** Enter the first part of your home postcode.

----

- **Screen:** Do you have a high temperature?

----

- **Screen:** When did you first start showing these symptoms?

----

- **Screen:** How this app works

### Android Accessibility Scanner

- No issues.

### Voice Access on Android

- **Screen:** Follow the current advice to stop the spread of coronavirus

### Zoomed on Android

- No issues.

### TalkBack on Android

- **Screen:** Help the NHS stop the spread of coronavirus in the UK

----

- **Screen:** Follow the current advice to stop the spread of coronavirus

----

- **Screen:** Follow the current advice to stop the spread of coronavirus

----

- **Screen:** Follow the current advice to stop the spread of coronavirus

### Test the service with various native settings on an iOS device

- **Screen:** Enter the first part of your home postcode

----

- **Screen:** Coronavirus tracing

----

- **Screen:** Do you have a high temperature?

----

- **Screen:** This app currently only works in the Isle of Wight

----

- **Screen:** Add my symptoms

----

- **Screen:** Diagnosis

----

### Xcode Accessibility Inspector

- **Screen:** Enter the first part of your home postcode

----

- **Screen:** Enter the first part of your home postcode

----

- **Screen:** Follow the current advice to stop the spread of coronavirus

----

- **Screen:** Follow the current advice to stop the spread of coronavirus

----

- **Screen:** Follow the current advice to stop the spread of coronavirus

----

- **Screen:** Follow the current advice to stop the spread of coronavirus

----

- **Screen:** Confirm the information

----

- **Screen:** Confirm the information

----

- **Screen:** Your symptoms indicate you may have coronavirus

----


### Voice Control on iOS

- No issues.

### Zoomed on iOS


### VoiceOver on iOS

----

- **Screen:** Enter the first part of your home postcode

### Test notifications

- Successful.

### Usability and performance

- **Screen:** Enter the first part of your home postcode

----

- **3.3.4 Error Prevention (Legal, Financial, Data)** Level AA
- **3.3.6 Error Prevention (All)** Level AAA
  - Reversible: Submissions are reversible.
  - Checked: Data entered by the user is checked for input errors and the user is provided an opportunity to correct them.
  - Confirmed: A mechanism is available for reviewing, confirming, and correcting information before finalizing the submission.

## Appendix I: Web Content Accessibility Guidelines (WCAG) 2.1

### Classification of Accessibility Issues

The following scoring system was used to indicate the status of the sites with regards to each W3C WAI checkpoint up to and including Level AAA

| Status                      | Description                                                                                                                                                                                             |
| --------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| 🟢 (P) Pass                  | The site meets the requirements of the checkpoint.                                                                                                                                                      |
| 🟣 (L) Fail: Low Priority    | The site almost meets the requirements of the checkpoint. Only a small number of minor problems were identified. The site fails to meet the requirements against AAA criteria measured against WCAG 2.1 |
| 🟠 (M) Fail: Medium Priority | The site fails to meet the requirements against AA criteria measured against WCAG 2.1                                                                                                                   |
| 🔴 (H) Fail: High Priority   | The site fails to meet the requirements against A criteria measured against WCAG 2.1 and more severe accessibility issues were identified.                                                              |
| ⚪️ (N/A) Not Applicable      | No content was found on the site to which the checkpoint would relate.                                                                                                                                  |

### Perceivable

Information and user interface components must be presentable to users in ways they can perceive.

#### Guideline 1.1 Text Alternatives

Provide text alternatives for any non-text content so that it can be changed into other forms people need, such as large print, braille, speech, symbols or simpler language.

| iOS   | Android | Level | Success Criterion                                                                  |
| ----- | ------- | ----- | ---------------------------------------------------------------------------------- |
| 🔴 (H) | 🟢 (P)   | A     | [1.1.1 Non-text Content](https://www.w3.org/WAI/WCAG21/quickref/#non-text-content) |

#### Guideline 1.2 Time-based Media

Provide alternatives for time-based media.

| iOS     | Android | Level | Success Criterion                                                                                                                                        |
| ------- | ------- | ----- | -------------------------------------------------------------------------------------------------------------------------------------------------------- |
| ⚪️ (N/A) | ⚪️ (N/A) | A     | [1.2.1 Audio-only and Video-only (Prerecorded)](https://www.w3.org/WAI/WCAG21/quickref/#audio-only-and-video-only-prerecorded)                           |
| ⚪️ (N/A) | ⚪️ (N/A) | A     | [1.2.2 Captions (Prerecorded)](https://www.w3.org/WAI/WCAG21/quickref/#captions-prerecorded)                                                             |
| ⚪️ (N/A) | ⚪️ (N/A) | A     | [1.2.3 Audio Description or Media Alternative (Prerecorded)](https://www.w3.org/WAI/WCAG21/quickref/#audio-description-or-media-alternative-prerecorded) |
| ⚪️ (N/A) | ⚪️ (N/A) | AA    | [1.2.4 Captions (Live)](https://www.w3.org/WAI/WCAG21/quickref/#captions-live)                                                                           |
| ⚪️ (N/A) | ⚪️ (N/A) | AA    | [1.2.5 Audio Description (Prerecorded)](https://www.w3.org/WAI/WCAG21/quickref/#audio-description-prerecorded)                                           |
| ⚪️ (N/A) | ⚪️ (N/A) | AAA   | [1.2.6 Sign Language (Prerecorded)](https://www.w3.org/WAI/WCAG21/quickref/#sign-language-prerecorded)                                                   |
| ⚪️ (N/A) | ⚪️ (N/A) | AAA   | [1.2.7 Extended Audio Description (Prerecorded)](https://www.w3.org/WAI/WCAG21/quickref/#extended-audio-description-prerecorded)                         |
| ⚪️ (N/A) | ⚪️ (N/A) | AAA   | [1.2.8 Media Alternative (Prerecorded)](https://www.w3.org/WAI/WCAG21/quickref/#media-alternative-prerecorded)                                           |
| ⚪️ (N/A) | ⚪️ (N/A) | AAA   | [1.2.9 Audio-only (Live)](https://www.w3.org/WAI/WCAG21/quickref/#audio-only-live)                                                                       |

#### Guideline 1.3 Adaptable

Create content that can be presented in different ways (for example simpler layout) without losing information or structure.

| iOS     | Android | Level | Success Criterion                                                                                             |
| ------- | ------- | ----- | ------------------------------------------------------------------------------------------------------------- |
| 🟢 (P)   | 🔴 (H)   | A     | [1.3.1 Info and Relationships](https://www.w3.org/WAI/WCAG21/quickref/#info-and-relationships)                |
| 🟢 (P)   | 🟢 (P)   | A     | [1.3.2 Meaningful Sequence](https://www.w3.org/WAI/WCAG21/quickref/#meaningful-sequence)                      |
| 🟢 (P)   | 🟢 (P)   | A     | [1.3.3 Sensory Characteristics](https://www.w3.org/WAI/WCAG21/quickref/#sensory-characteristics)              |
| 🟢 (P)   | 🟢 (P)   | AA    | [1.3.4 Orientation](https://www.w3.org/WAI/WCAG21/quickref/#orientation) (Added in 2.1)                       |
| ⚪️ (N/A) | ⚪️ (N/A) | AA    | [1.3.5 Identify Input Purpose](https://www.w3.org/WAI/WCAG21/quickref/#identify-input-purpose) (Added in 2.1) |
| ⚪️ (N/A) | ⚪️ (N/A) | AAA   | [1.3.6 Identify Purpose](https://www.w3.org/WAI/WCAG21/quickref/#identify-purpose) (Added in 2.1)             |

#### Guideline 1.4 Distinguishable

Make it easier for users to see and hear content including separating foreground from background.

| iOS     | Android | Level | Success Criterion                                                                                                    |
| ------- | ------- | ----- | -------------------------------------------------------------------------------------------------------------------- |
| 🔴 (H)   | 🔴 (H)   | A     | [1.4.1 Use of Color](https://www.w3.org/WAI/WCAG21/quickref/#use-of-color)                                           |
| ⚪️ (N/A) | ⚪️ (N/A) | A     | [1.4.2 Audio Control](https://www.w3.org/WAI/WCAG21/quickref/#audio-control)                                         |
| 🟠 (M)   | 🟠 (M)   | AA    | [1.4.3 Contrast (Minimum)](https://www.w3.org/WAI/WCAG21/quickref/#contrast-minimum)                                 |
| 🟠 (M)   | 🟠 (M)   | AA    | [1.4.4 Resize text](https://www.w3.org/WAI/WCAG21/quickref/#resize-text)                                             |
| 🟢 (P)   | 🟢 (P)   | AA    | [1.4.5 Images of Text](https://www.w3.org/WAI/WCAG21/quickref/#images-of-text)                                       |
| ⚪️ (N/A) | ⚪️ (N/A) | AAA   | [1.4.6 Contrast (Enhanced)](https://www.w3.org/WAI/WCAG21/quickref/#contrast-enhanced)                               |
| ⚪️ (N/A) | ⚪️ (N/A) | AAA   | [1.4.7 Low or No Background Audio](https://www.w3.org/WAI/WCAG21/quickref/#low-or-no-background-audio)               |
| ⚪️ (N/A) | ⚪️ (N/A) | AAA   | [1.4.8 Visual Presentation](https://www.w3.org/WAI/WCAG21/quickref/#visual-presentation)                             |
| ⚪️ (N/A) | ⚪️ (N/A) | AAA   | [1.4.9 Images of Text (No Exception)](https://www.w3.org/WAI/WCAG21/quickref/#images-of-text-no-exception)           |
| ⚪️ (N/A) | ⚪️ (N/A) | AA    | [1.4.10 Reflow](https://www.w3.org/WAI/WCAG21/quickref/#reflow) (Added in 2.1)                                       |
| ⚪️ (N/A) | ⚪️ (N/A) | AA    | [1.4.11 Non-text Contrast](https://www.w3.org/WAI/WCAG21/quickref/#non-text-contrast) (Added in 2.1)                 |
| ⚪️ (N/A) | ⚪️ (N/A) | AA    | [1.4.12 Text Spacing](https://www.w3.org/WAI/WCAG21/quickref/#text-spacing) (Added in 2.1)                           |
| ⚪️ (N/A) | ⚪️ (N/A) | AA    | [1.4.13 Content on Hover or Focus](https://www.w3.org/WAI/WCAG21/quickref/#content-on-hover-or-focus) (Added in 2.1) |

### Operable

User interface components and navigation must be operable.

#### Guideline 2.1 Keyboard Accessible

Make all functionality available from a keyboard.

| iOS     | Android | Level | Success Criterion                                                                                               |
| ------- | ------- | ----- | --------------------------------------------------------------------------------------------------------------- |
| 🟢 (P)   | 🟢 (P)   | A     | [2.1.1 Keyboard](https://www.w3.org/WAI/WCAG21/quickref/#keyboard)                                              |
| 🟢 (P)   | 🟢 (P)   | A     | [2.1.2 No Keyboard Trap](https://www.w3.org/WAI/WCAG21/quickref/#no-keyboard-trap)                              |
| ⚪️ (N/A) | ⚪️ (N/A) | AAA   | [2.1.3 Keyboard (No Exception)](https://www.w3.org/WAI/WCAG21/quickref/#keyboard-no-exception)                  |
| ⚪️ (N/A) | ⚪️ (N/A) | A     | [2.1.4 Character Key Shortcuts](https://www.w3.org/WAI/WCAG21/quickref/#character-key-shortcuts) (Added in 2.1) |

#### Guideline 2.2 Enough Time

Provide users enough time to read and use content.

| iOS     | Android | Level | Success Criterion                                                                    |
| ------- | ------- | ----- | ------------------------------------------------------------------------------------ |
| ⚪️ (N/A) | ⚪️ (N/A) | A     | [2.2.1 Timing Adjustable](https://www.w3.org/WAI/WCAG21/quickref/#timing-adjustable) |
| ⚪️ (N/A) | ⚪️ (N/A) | A     | [2.2.2 Pause, Stop, Hide](https://www.w3.org/WAI/WCAG21/quickref/#pause-stop-hide)   |
| ⚪️ (N/A) | ⚪️ (N/A) | AAA   | [2.2.3 No Timing](https://www.w3.org/WAI/WCAG21/quickref/#no-timing)                 |
| ⚪️ (N/A) | ⚪️ (N/A) | AAA   | [2.2.4 Interruptions](https://www.w3.org/WAI/WCAG21/quickref/#interruptions)         |
| ⚪️ (N/A) | ⚪️ (N/A) | AAA   | [2.2.5 Re-authenticating](https://www.w3.org/WAI/WCAG21/quickref/#re-authenticating) |
| ⚪️ (N/A) | ⚪️ (N/A) | AAA   | [2.2.6 Timeouts](https://www.w3.org/WAI/WCAG21/quickref/#timeouts) (Added in 2.1)    |

#### Guideline 2.3 Seizures and Physical Reactions

Do not design content in a way that is known to cause seizures or physical reactions.

| iOS     | Android | Level | Success Criterion                                                                                                       |
| ------- | ------- | ----- | ----------------------------------------------------------------------------------------------------------------------- |
| ⚪️ (N/A) | ⚪️ (N/A) | A     | [2.3.1 Three Flashes or Below Threshold](https://www.w3.org/WAI/WCAG21/quickref/#three-flashes-or-below-threshold)      |
| ⚪️ (N/A) | ⚪️ (N/A) | AAA   | [2.3.2 Three Flashes](https://www.w3.org/WAI/WCAG21/quickref/#three-flashes)                                            |
| ⚪️ (N/A) | ⚪️ (N/A) | AAA   | [2.3.3 Animation from Interactions](https://www.w3.org/WAI/WCAG21/quickref/#animation-from-interactions) (Added in 2.1) |

#### Guideline 2.4 Navigable

Provide ways to help users navigate, find content, and determine where they are.

| iOS     | Android | Level | Success Criterion                                                                                  |
| ------- | ------- | ----- | -------------------------------------------------------------------------------------------------- |
| ⚪️ (N/A) | ⚪️ (N/A) | A     | [2.4.1 Bypass Blocks](https://www.w3.org/WAI/WCAG21/quickref/#bypass-blocks)                       |
| 🔴 (H)   | 🔴 (H)   | A     | [2.4.2 Page Titled](https://www.w3.org/WAI/WCAG21/quickref/#page-titled)                           |
| 🟢 (P)   | 🟢 (P)   | A     | [2.4.3 Focus Order](https://www.w3.org/WAI/WCAG21/quickref/#focus-order)                           |
| 🟣 (L)   | 🟢 (P)   | A     | [2.4.4 Link Purpose (In Context)](https://www.w3.org/WAI/WCAG21/quickref/#link-purpose-in-context) |
| ⚪️ (N/A) | ⚪️ (N/A) | AA    | [2.4.5 Multiple Ways](https://www.w3.org/WAI/WCAG21/quickref/#multiple-ways)                       |
| 🟠 (M)   | 🟠 (M)   | AA    | [2.4.6 Headings and Labels](https://www.w3.org/WAI/WCAG21/quickref/#headings-and-labels)           |
| 🟠 (M)   | 🟠 (M)   | AA    | [2.4.7 Focus Visible](https://www.w3.org/WAI/WCAG21/quickref/#focus-visible)                       |
| ⚪️ (N/A) | ⚪️ (N/A) | AAA   | [2.4.8 Location](https://www.w3.org/WAI/WCAG21/quickref/#location)                                 |
| 🟣 (L)   | 🟢 (P)   | AAA   | [2.4.9 Link Purpose (Link Only)](https://www.w3.org/WAI/WCAG21/quickref/#link-purpose-link-only)   |
| 🟣 (L)   | 🟣 (L)   | AAA   | [2.4.10 Section Headings](https://www.w3.org/WAI/WCAG21/quickref/#section-headings)                |

#### Guideline 2.5 Input Modalities

Make it easier for users to operate functionality through various inputs beyond keyboard.

| iOS     | Android | Level | Success Criterion                                                                                                       |
| ------- | ------- | ----- | ----------------------------------------------------------------------------------------------------------------------- |
| 🟢 (P)   | 🟢 (P)   | A     | [2.5.1 Pointer Gestures](https://www.w3.org/WAI/WCAG21/quickref/#pointer-gestures) (Added in 2.1)                       |
| 🟢 (P)   | 🟢 (P)   | A     | [2.5.2 Pointer Cancellation](https://www.w3.org/WAI/WCAG21/quickref/#pointer-cancellation) (Added in 2.1)               |
| ⚪️ (N/A) | ⚪️ (N/A) | A     | [2.5.3 Label in Name](https://www.w3.org/WAI/WCAG21/quickref/#label-in-name) (Added in 2.1)                             |
| ⚪️ (N/A) | ⚪️ (N/A) | A     | [2.5.4 Motion Actuation](https://www.w3.org/WAI/WCAG21/quickref/#motion-actuation) (Added in 2.1)                       |
| 🟣 (L)   | 🟢 (P)   | AAA   | [2.5.5 Target Size](https://www.w3.org/WAI/WCAG21/quickref/#target-size) (Added in 2.1)                                 |
| ⚪️ (N/A) | ⚪️ (N/A) | AAA   | [2.5.6 Concurrent Input Mechanisms](https://www.w3.org/WAI/WCAG21/quickref/#concurrent-input-mechanisms) (Added in 2.1) |

### Understandable

Information and the operation of user interface must be understandable.

#### Guideline 3.1 Readable

Make text content readable and understandable.

| iOS   | Android | Level | Success Criterion                                                                    |
| ----- | ------- | ----- | ------------------------------------------------------------------------------------ |
| 🟢 (P) | 🟢 (P)   | A     | [3.1.1 Language of Page](https://www.w3.org/WAI/WCAG21/quickref/#language-of-page)   |
| 🟢 (P) | 🟢 (P)   | AA    | [3.1.2 Language of Parts](https://www.w3.org/WAI/WCAG21/quickref/#language-of-parts) |
| 🟢 (P) | 🟢 (P)   | AAA   | [3.1.3 Unusual Words](https://www.w3.org/WAI/WCAG21/quickref/#unusual-words)         |
| 🟢 (P) | 🟢 (P)   | AAA   | [3.1.4 Abbreviations](https://www.w3.org/WAI/WCAG21/quickref/#abbreviations)         |
| 🟢 (P) | 🟢 (P)   | AAA   | [3.1.5 Reading Level](https://www.w3.org/WAI/WCAG21/quickref/#reading-level)         |
| 🟢 (P) | 🟢 (P)   | AAA   | [3.1.6 Pronunciation](https://www.w3.org/WAI/WCAG21/quickref/#pronunciation)         |

#### Guideline 3.2 Predictable

Make Web pages appear and operate in predictable ways.

| iOS   | Android | Level | Success Criterion                                                                                    |
| ----- | ------- | ----- | ---------------------------------------------------------------------------------------------------- |
| 🟢 (P) | 🟢 (P)   | A     | [3.2.1 On Focus](https://www.w3.org/WAI/WCAG21/quickref/#on-focus)                                   |
| 🟢 (P) | 🟢 (P)   | A     | [3.2.2 On Input](https://www.w3.org/WAI/WCAG21/quickref/#on-input)                                   |
| 🟢 (P) | 🟢 (P)   | AA    | [3.2.3 Consistent Navigation](https://www.w3.org/WAI/WCAG21/quickref/#consistent-navigation)         |
| 🟢 (P) | 🟢 (P)   | AA    | [3.2.4 Consistent Identification](https://www.w3.org/WAI/WCAG21/quickref/#consistent-identification) |
| 🟢 (P) | 🟢 (P)   | AAA   | [3.2.5 Change on Request](https://www.w3.org/WAI/WCAG21/quickref/#change-on-request)                 |

#### Guideline 3.3 Input Assistance

Help users avoid and correct mistakes.

| iOS     | Android | Level | Success Criterion                                                                                                                |
| ------- | ------- | ----- | -------------------------------------------------------------------------------------------------------------------------------- |
| 🔴 (H)   | 🔴 (H)   | A     | [3.3.1 Error Identification](https://www.w3.org/WAI/WCAG21/quickref/#error-identification)                                       |
| 🟢 (P)   | 🟢 (P)   | A     | [3.3.2 Labels or Instructions](https://www.w3.org/WAI/WCAG21/quickref/#labels-or-instructions)                                   |
| 🟢 (P)   | 🟢 (P)   | AA    | [3.3.3 Error Suggestion](https://www.w3.org/WAI/WCAG21/quickref/#error-suggestion)                                               |
| 🟠 (M)   | 🟠 (M)   | AA    | [3.3.4 Error Prevention (Legal, Financial, Data)](https://www.w3.org/WAI/WCAG21/quickref/#error-prevention-legal-financial-data) |
| ⚪️ (N/A) | ⚪️ (N/A) | AAA   | [3.3.5 Help](https://www.w3.org/WAI/WCAG21/quickref/#help)                                                                       |
| 🟣 (L)   | 🟣 (L)   | AAA   | [3.3.6 Error Prevention (All)](https://www.w3.org/WAI/WCAG21/quickref/#error-prevention-all)                                     |

### Robust

Content must be robust enough that it can be interpreted by by a wide variety of user agents, including assistive technologies.

#### Guideline 4.1 Compatible

Maximize compatibility with current and future user agents, including assistive technologies.

| iOS     | Android | Level | Success Criterion                                                                               |
| ------- | ------- | ----- | ----------------------------------------------------------------------------------------------- |
| ⚪️ (N/A) | ⚪️ (N/A) | A     | [4.1.1 Parsing](https://www.w3.org/WAI/WCAG21/quickref/#parsing)                                |
| 🟢 (P)   | 🔴 (H)   | A     | [4.1.2 Name, Role, Value](https://www.w3.org/WAI/WCAG21/quickref/#name-role-value)              |
| 🟢 (P)   | 🟢 (P)   | AA    | [4.1.3 Status Messages](https://www.w3.org/WAI/WCAG21/quickref/#status-messages) (Added in 2.1) |

## Appendix II: Accessibility Criteria


## Appendix III: Reference

- [Understanding WCAG 2.1](https://www.w3.org/WAI/WCAG21/Understanding)
- [Techniques for WCAG 2.1](https://www.w3.org/WAI/WCAG21/Techniques)
- [How to Meet WCAG (Quick Reference)](https://www.w3.org/WAI/WCAG21/quickref/)
- [Supporting VoiceOver in Your App](https://developer.apple.com/documentation/uikit/accessibility/supporting_voiceover_in_your_app)

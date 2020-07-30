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

- iOS build #
- Android build #

## Executive summary

An accessibility report for the NHSx COVID-19 mobile application. The application was assessed against WCAG 2 Mobile Accessibility Guidelines. Full details below in [Appendix I: WCAG 2 Mobile Accessibility Guidelines].

The following violations need fixing in order to comply.

| Platform | Level | Success Criterion                               |
| -------- | ----- | ----------------------------------------------- |
| iOS      | 🔴 (H) | 1.1.1 Non-text Content                          |
| Android  | 🔴 (H) | 1.3.1 Info and Relationships                    |
| Both     | 🟠 (M) | 1.4.3 Contrast (Minimum)                        |


## Accessibility test results

### Classification of Issues

The following scoring system was used to indicate the status of the app with regards to each WCAG 2.0 AA Guidelines

| Status                      | Description                                                                                                                                                                                             |
| --------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| 🟢 (P) Pass                  | The app meets the requirement                                                                                                                                                   |
| 🔴 (H) Fail:                  | The app fails to meet the requirement                                                              |
| ⚪️ (N/A) Not Applicable       | No relevant content was found                                                                                 |

### 1 Perceivable
Information and user interface components must be presentable to users in ways they can perceive.

#### 1.1 Text Alternatives
Provide text alternatives for any non-text content so that it can be changed into other forms people need, such as large print, braille, speech, symbols or simpler language.

| iOS   | Android | Level | Success Criterion                                                                  |
| ----- | ------- | ----- | ---------------------------------------------------------------------------------- |
| 🔴 (H) | 🟢 (P)   | A     | [1.1.1 Non-text Content](https://www.w3.org/WAI/WCAG21/quickref/#non-text-content) |

#### 1.2 Time-based Media
Provide alternatives for time-based media.

| iOS     | Android | Level | Success Criterion                                                                                                                                        |
| ------- | ------- | ----- | -------------------------------------------------------------------------------------------------------------------------------------------------------- |
| ⚪️ (N/A) | ⚪️ (N/A) | A     | [1.2.1 Audio-only and Video-only (Prerecorded)](https://www.w3.org/WAI/WCAG21/quickref/#audio-only-and-video-only-prerecorded)                           |
| ⚪️ (N/A) | ⚪️ (N/A) | A     | [1.2.2 Captions (Prerecorded)](https://www.w3.org/WAI/WCAG21/quickref/#captions-prerecorded)                                                             |
| ⚪️ (N/A) | ⚪️ (N/A) | A     | [1.2.3 Audio Description or Media Alternative (Prerecorded)](https://www.w3.org/WAI/WCAG21/quickref/#audio-description-or-media-alternative-prerecorded) |
| ⚪️ (N/A) | ⚪️ (N/A) | AA    | [1.2.4 Captions (Live)](https://www.w3.org/WAI/WCAG21/quickref/#captions-live)                                                                           |
| ⚪️ (N/A) | ⚪️ (N/A) | AA    | [1.2.5 Audio Description (Prerecorded)](https://www.w3.org/WAI/WCAG21/quickref/#audio-description-prerecorded)                                           |

#### 1.3 Adaptable
Create content that can be presented in different ways (for example simpler layout) without losing information or structure.

| iOS     | Android | Level | Success Criterion                                                                                             |
| ------- | ------- | ----- | ------------------------------------------------------------------------------------------------------------- |
| 🟢 (P)   | 🔴 (H)   | A     | [1.3.1 Info and Relationships](https://www.w3.org/WAI/WCAG21/quickref/#info-and-relationships)                |
| 🟢 (P)   | 🟢 (P)   | A     | [1.3.2 Meaningful Sequence](https://www.w3.org/WAI/WCAG21/quickref/#meaningful-sequence)                      |
| 🟢 (P)   | 🟢 (P)   | A     | [1.3.3 Sensory Characteristics](https://www.w3.org/WAI/WCAG21/quickref/#sensory-characteristics)              |
| 🟢 (P)   | 🟢 (P)   | AA    | [1.3.4 Orientation](https://www.w3.org/WAI/WCAG21/quickref/#orientation) (Added in 2.1)                       |
| ⚪️ (N/A) | ⚪️ (N/A) | AA    | [1.3.5 Identify Input Purpose](https://www.w3.org/WAI/WCAG21/quickref/#identify-input-purpose) (Added in 2.1) |

#### 1.4 Distinguishable
Make it easier for users to see and hear content including separating foreground from background.

| iOS     | Android | Level | Success Criterion                                                                                                    |
| ------- | ------- | ----- | -------------------------------------------------------------------------------------------------------------------- |
| 🔴 (H)   | 🔴 (H)   | A     | [1.4.1 Use of Color](https://www.w3.org/WAI/WCAG21/quickref/#use-of-color)                                           |
| ⚪️ (N/A) | ⚪️ (N/A) | A     | [1.4.2 Audio Control](https://www.w3.org/WAI/WCAG21/quickref/#audio-control)                                         |
| 🟠 (M)   | 🟠 (M)   | AA    | [1.4.3 Contrast (Minimum)](https://www.w3.org/WAI/WCAG21/quickref/#contrast-minimum)                                 |
| 🟠 (M)   | 🟠 (M)   | AA    | [1.4.4 Resize text](https://www.w3.org/WAI/WCAG21/quickref/#resize-text)                                             |
| 🟢 (P)   | 🟢 (P)   | AA    | [1.4.5 Images of Text](https://www.w3.org/WAI/WCAG21/quickref/#images-of-text)                                       |
| ⚪️ (N/A) | ⚪️ (N/A) | AA    | [1.4.10 Reflow](https://www.w3.org/WAI/WCAG21/quickref/#reflow) (Added in 2.1)                                       |
| ⚪️ (N/A) | ⚪️ (N/A) | AA    | [1.4.11 Non-text Contrast](https://www.w3.org/WAI/WCAG21/quickref/#non-text-contrast) (Added in 2.1)                 |
| ⚪️ (N/A) | ⚪️ (N/A) | AA    | [1.4.12 Text Spacing](https://www.w3.org/WAI/WCAG21/quickref/#text-spacing) (Added in 2.1)                           |
| ⚪️ (N/A) | ⚪️ (N/A) | AA    | [1.4.13 Content on Hover or Focus](https://www.w3.org/WAI/WCAG21/quickref/#content-on-hover-or-focus) (Added in 2.1) |

### 2 Operable
User interface components and navigation must be operable.

#### 2.1 Keyboard Accessible
Make all functionality available from a keyboard.

| iOS     | Android | Level | Success Criterion                                                                                               |
| ------- | ------- | ----- | --------------------------------------------------------------------------------------------------------------- |
| 🟢 (P)   | 🟢 (P)   | A     | [2.1.1 Keyboard](https://www.w3.org/WAI/WCAG21/quickref/#keyboard)                                              |
| 🟢 (P)   | 🟢 (P)   | A     | [2.1.2 No Keyboard Trap](https://www.w3.org/WAI/WCAG21/quickref/#no-keyboard-trap)                              |
| ⚪️ (N/A) | ⚪️ (N/A) | A     | [2.1.4 Character Key Shortcuts](https://www.w3.org/WAI/WCAG21/quickref/#character-key-shortcuts) (Added in 2.1) |

#### 2.2 Enough Time
Provide users enough time to read and use content.

| iOS     | Android | Level | Success Criterion                                                                    |
| ------- | ------- | ----- | ------------------------------------------------------------------------------------ |
| ⚪️ (N/A) | ⚪️ (N/A) | A     | [2.2.1 Timing Adjustable](https://www.w3.org/WAI/WCAG21/quickref/#timing-adjustable) |
| ⚪️ (N/A) | ⚪️ (N/A) | A     | [2.2.2 Pause, Stop, Hide](https://www.w3.org/WAI/WCAG21/quickref/#pause-stop-hide)   |

### 2.3 Seizures and Physical Reactions
Do not design content in a way that is known to cause seizures or physical reactions.

| iOS     | Android | Level | Success Criterion                                                                                                       |
| ------- | ------- | ----- | ----------------------------------------------------------------------------------------------------------------------- |
| ⚪️ (N/A) | ⚪️ (N/A) | A     | [2.3.1 Three Flashes or Below Threshold](https://www.w3.org/WAI/WCAG21/quickref/#three-flashes-or-below-threshold)      |

### 2.4 Navigable
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

#### 2.5 Input Modalities
Make it easier for users to operate functionality through various inputs beyond keyboard.

| iOS     | Android | Level | Success Criterion                                                                                                       |
| ------- | ------- | ----- | ----------------------------------------------------------------------------------------------------------------------- |
| 🟢 (P)   | 🟢 (P)   | A     | [2.5.1 Pointer Gestures](https://www.w3.org/WAI/WCAG21/quickref/#pointer-gestures) (Added in 2.1)                       |
| 🟢 (P)   | 🟢 (P)   | A     | [2.5.2 Pointer Cancellation](https://www.w3.org/WAI/WCAG21/quickref/#pointer-cancellation) (Added in 2.1)               |
| ⚪️ (N/A) | ⚪️ (N/A) | A     | [2.5.3 Label in Name](https://www.w3.org/WAI/WCAG21/quickref/#label-in-name) (Added in 2.1)                             |
| ⚪️ (N/A) | ⚪️ (N/A) | A     | [2.5.4 Motion Actuation](https://www.w3.org/WAI/WCAG21/quickref/#motion-actuation) (Added in 2.1)                       |

### 3 Understandable
Information and the operation of user interface must be understandable.

#### 3.1 Readable
Make text content readable and understandable.

| iOS   | Android | Level | Success Criterion                                                                    |
| ----- | ------- | ----- | ------------------------------------------------------------------------------------ |
| 🟢 (P) | 🟢 (P)   | A     | [3.1.1 Language of Page](https://www.w3.org/WAI/WCAG21/quickref/#language-of-page)   |
| 🟢 (P) | 🟢 (P)   | AA    | [3.1.2 Language of Parts](https://www.w3.org/WAI/WCAG21/quickref/#language-of-parts) |

#### 3.2 Predictable
Make Web pages appear and operate in predictable ways.

| iOS   | Android | Level | Success Criterion                                                                                    |
| ----- | ------- | ----- | ---------------------------------------------------------------------------------------------------- |
| 🟢 (P) | 🟢 (P)   | A     | [3.2.1 On Focus](https://www.w3.org/WAI/WCAG21/quickref/#on-focus)                                   |
| 🟢 (P) | 🟢 (P)   | A     | [3.2.2 On Input](https://www.w3.org/WAI/WCAG21/quickref/#on-input)                                   |
| 🟢 (P) | 🟢 (P)   | AA    | [3.2.3 Consistent Navigation](https://www.w3.org/WAI/WCAG21/quickref/#consistent-navigation)         |
| 🟢 (P) | 🟢 (P)   | AA    | [3.2.4 Consistent Identification](https://www.w3.org/WAI/WCAG21/quickref/#consistent-identification) |

#### 3.3 Input Assistance
Help users avoid and correct mistakes.

| iOS     | Android | Level | Success Criterion                                                                                                                |
| ------- | ------- | ----- | -------------------------------------------------------------------------------------------------------------------------------- |
| 🔴 (H)   | 🔴 (H)   | A     | [3.3.1 Error Identification](https://www.w3.org/WAI/WCAG21/quickref/#error-identification)                                       |
| 🟢 (P)   | 🟢 (P)   | A     | [3.3.2 Labels or Instructions](https://www.w3.org/WAI/WCAG21/quickref/#labels-or-instructions)                                   |
| 🟢 (P)   | 🟢 (P)   | AA    | [3.3.3 Error Suggestion](https://www.w3.org/WAI/WCAG21/quickref/#error-suggestion)                                               |
| 🟠 (M)   | 🟠 (M)   | AA    | [3.3.4 Error Prevention (Legal, Financial, Data)](https://www.w3.org/WAI/WCAG21/quickref/#error-prevention-legal-financial-data) |

### Robust
Content must be robust enough that it can be interpreted by by a wide variety of user agents, including assistive technologies.

#### 4.1 Compatible 
Maximize compatibility with current and future user agents, including assistive technologies.

| iOS     | Android | Level | Success Criterion                                                                               |
| ------- | ------- | ----- | ----------------------------------------------------------------------------------------------- |
| ⚪️ (N/A) | ⚪️ (N/A) | A     | [4.1.1 Parsing](https://www.w3.org/WAI/WCAG21/quickref/#parsing)                                |
| 🟢 (P)   | 🔴 (H)   | A     | [4.1.2 Name, Role, Value](https://www.w3.org/WAI/WCAG21/quickref/#name-role-value)              |
| 🟢 (P)   | 🟢 (P)   | AA    | [4.1.3 Status Messages](https://www.w3.org/WAI/WCAG21/quickref/#status-messages) (Added in 2.1) |

## Appendix: Reference

- [Mobile Accessibility: How WCAG 2.0 and other W3C/WAI Guidelines Appply to Mobile](https://www.w3.org/TR/mobile-accessibility-mapping)
-[WCAG 2.0 Techniques that Apply to Mobile](https://www.w3.org/WAI/GL/mobile-a11y-tf/MobileTechniques)
- [How to Meet WCAG (Quick Reference)](https://www.w3.org/WAI/WCAG21/quickref)

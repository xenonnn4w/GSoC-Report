![GSoC logo](https://developers.google.com/open-source/gsoc/resources/downloads/GSoC-logo-horizontal.svg)

<h1 align="center">Anoop<br>2024 <br> 
  <a href="[AnkiDroid](https://github.com/ankidroid/Anki-Android)">AnkiDroid</a> </h1>

## My mentors
[David Allison](https://github.com/david-allison) | [Arthur Milchior](https://github.com/Arthur-Milchior)

## Project Details

[AnkiDroid](https://github.com/ankidroid/Anki-Android) is a companion Android application for [Anki](https://github.com/ankitects/anki), a 
flashcards application that helps people learn and memorize a diverse variety of topics. 

[Additional Widgets](https://summerofcode.withgoogle.com/programs/2024/projects/w1n3pqnM) is mainly about
* Introducing the Deck Picker Widget.
  <p align="center">
    <img alt="" src="files/DeckPicker.png" width="30%" height="30%">
  </p>
* Introducing the Card Analysis Widget.
    <p align="center">
    <img alt="" src="files/CardAnalysis.png" width="30%" height="30%">
    </p>


### Deck Picker Widget
The Deck Picker Widget offers users a convenient display of their decks, showcasing the number of cards that are new, in learning, and due for review, all at a glance. This display-only widget allows users to quickly review any deck by simply clicking on it directly from the widget. With a maximum of five decks that can be selected, users can reconfigure their widget by holding it down, making it easy to customize their overview. This feature-rich widget provides a seamless way for users to stay on top of their study progress without having to open the app.
<p align="center">
    <video width="500px" 
           height="400px" 
           controls="controls">
        <source src="files/DeckPickerVideo" video/mp4" />
    </video>
</p>
### After Instant Note Editor
Users can select and share selected text to AnkiDroid. The `Instant Note` feature helps them create cloze notes without actually opening the app:
<p align="center">
    <img alt="" src="media/cloze-editor.png" width="30%" height="30%">   
    <img alt="" src="media/clozed-words.png" width="30%" height="30%">
    <img alt="" src="media/advance-edit.png" width="30%" height="30%">
</p>

### Old Multimedia UI
<p align="center">
    <img alt="" src="media/mm_o.png" width="30%" height="30%">
    <img alt="" src="media/mm_oi.png" width="30%" height="30%">
</p>

### New Multimedia UI
<p align="center">
    <img alt="" src="media/mm_b.png" width="30%" height="30%">
    <img alt="" src="media/mm_i.png" width="30%" height="30%">
</p>

## Working

### Instant Note Editor
<p align="center">
    <img alt="" src="media/instant_editor.png">
</p>

### Multimedia UI/UX
<p align="center">
    <img alt="" src="media/multimedia.png">
</p>

## How did I do it?

### Community Bonding Period
Community Bonding is the initial time that Google gives to be involved in the community and activities that happen within an organization. Since the community was small and I already had been contributing and knew the community, it went very well. I enjoyed it and started my coding during this period so that I could compensate for the time that I wouldn't be active due to my university exams.

### Instant Note Editor
During the first phase of the GSoC project, the development of the Instant Note Editor was a key focus. The journey started with establishing foundational elements like design resources and intent filters, followed by creating a preliminary layout for the editor dialog. Over the subsequent weeks, the project saw rapid progress, with significant enhancements to both the user interface and functionality.

Key milestones included implementing `ActionMode.Callback` for better context menu handling, refining error validation, and migrating business logic to ViewModel for improved state management. A crucial improvement in the user interface was the transition from using EditText with `Chip` drawables to `ChipGroup`. Initially, the use of `Chip` drawables within EditText presented challenges, such as difficulties in interacting with the chips independently and tracking them effectively. This limitation prompted a shift to ChipGroup, which allowed for independent interaction with words and the addition of badges on chips, leading to a more robust and flexible user experience.

The phase culminated in the finalization of the Instant Note Editor, which was then prepared for a controlled release cycle to ensure a polished and user-friendly public rollout.

### Multimedia UI/UX
The second phase of the project centered around the development of the Multimedia UI/UX, aiming to enrich the note-taking experience by integrating multimedia elements. The setup of the Multimedia activity marked the beginning of this phase, laying the groundwork for subsequent features. Over the weeks, the multimedia editor evolved to include options for camera and gallery integration, enabling users to seamlessly add images to their notes. The development was methodical, with features being tested and refined in a developer-only environment to ensure stability. As the project neared completion, additional multimedia options like audio recording and drawing were incorporated, further enhancing the user experience. The project was wrapped up with the Multimedia UI/UX being marked ready for public use, ensuring a robust and dynamic addition to the note editor.


## Link to pull requests created as a part of GSoC by chronological order
 1. [Instant Note Editor to allow adding cloze card](https://github.com/ankidroid/Anki-Android/pull/16393)
 2. [Extract ActionMode.Callback from NoteEditor](https://github.com/ankidroid/Anki-Android/pull/16401)
 3. [Extension method to get cloze field name](https://github.com/ankidroid/Anki-Android/pull/16424)
 4. [Ese field check from backend and display error accordingly](https://github.com/ankidroid/Anki-Android/pull/16432)
 5. [Init: Instant Note Editor Activity](https://github.com/ankidroid/Anki-Android/pull/16497)
 6. [Enhancements: Instant Note Editor Improvements](https://github.com/ankidroid/Anki-Android/pull/16534)
 7. [New Multimedia UI](https://github.com/ankidroid/Anki-Android/pull/16673)
 8. [Enhancement: add long press listener on cloze button ](https://github.com/ankidroid/Anki-Android/pull/16735)
 9. [Refactor: cloze builder pattern for words](https://github.com/ankidroid/Anki-Android/pull/16736)
 10. [Refactor: use prefill value in integer dialog](https://github.com/ankidroid/Anki-Android/pull/16745)
 11. [Enable instant editor for public use](https://github.com/ankidroid/Anki-Android/pull/16760)
 12. [Enhacement: add Audio and Video multimedia options](https://github.com/ankidroid/Anki-Android/pull/16769)
 13. [Fix: cloze number incorrect on undo](https://github.com/ankidroid/Anki-Android/pull/16779)
 14. [Refactor: Multimedia options converted to sealed class](https://github.com/ankidroid/Anki-Android/pull/16796) *Closed after discussion*
 15. [Multimedia UI/UX: Add Drawing & Recording options and set multimedia public](https://github.com/ankidroid/Anki-Android/pull/16798)
 16. [Refactor: vibration methods to use Duration](https://github.com/ankidroid/Anki-Android/pull/16803)
 17. [Refactor: move audio package to multimedia package ](https://github.com/ankidroid/Anki-Android/pull/16816)

## Plans after GSoC?
Having successfully fulfilled all the commitments outlined in my GSoC proposal, my focus now shifts towards further enhancing the quality and robustness of the codebase. One critical area that I plan to address is the creation of comprehensive test suites, including both Unit Tests and Android Tests. These tests are essential for ensuring the reliability and stability of the application, and I intend to develop them as part of my ongoing contributions to the project.

My journey with AnkiDroid does not end with the conclusion of GSoC. I am committed to continuing my involvement with the project, and leveraging the experience and knowledge I have gained to make meaningful contributions. By staying actively engaged with the AnkiDroid community, I aim to help maintain and improve the app, ensuring it continues to be a valuable tool for users worldwide.


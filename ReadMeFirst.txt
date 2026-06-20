CPACC - OpenDoorAccessibilityLab V1.3.8

This is a test build of the CPACC practice Lab.

Current focus:
- Domain 1 - Disability Models and Disability Experience
- Reinforce Mode
- Practice Mode
- Challenge Mode
- Sprint Mode
- Review Missed Questions

Testing notes:
- Sprint Mode gives results only at the end.
- Q repeats the current question.
- R announces remaining sprint time.
- Number keys 1 through 4 answer during Sprint.
- Escape ends Sprint early.
- Review Missed Questions appears after a session if any questions were answered incorrectly.

Known future work:
- Expand Domain 2.
- Add more domain questions.
- Improve long-term statistics.
- Add review missed question persistence across future sessions.

V1.3.13 notes:
- Review missed questions now announces the full review item after Alt+M, Next, and Previous.


V1.4.0 Update:
Domain 2 - Disability Demographics and Diversity is now enabled with 100 starter questions.


V1.4.2 Update:
- Added a dedicated Review Complete screen after missed-question review.
- Reworked Keyboard Shortcuts help into grouped lists using Focus Mode and Browse Mode language.
- Added Start New Session, Open Statistics, and Return Home flow after review completion.
\n\nV1.4.3 Update:\n- Cleaned Review Complete flow.\n- Review completion now has its own action area with Start New Session, Open Statistics, and Return Home.\n- Removed leftover Finish Review, Previous Missed Question, and Session Review controls from the completion state.\n

V1.4.4 Update:
- Finalized Review Complete workflow.
- Review Complete now hides stale quiz and review controls.
- Focus lands on Start New Session after review completion.
- Final action tab order is Start New Session, Open Statistics, Return Home.


V1.4.5 Update:
- Replaced Keyboard Shortcuts with Getting Started and Keyboard Tips.
- Added Focus Mode/Browse Mode guidance.
- Added persistent collapsed state for the instructions disclosure.
- Escape now collapses the Getting Started section and returns focus to the summary button.


V1.4.6 Update:
- Restored answer challenge workflow during missed-question review.
- Added Proposed answer, Reasoning for instructor review, Save Challenge, and Export Challenges for Instructor Review.


V1.4.7 Update:
- Moved Challenge This Answer into a collapsed details element during review.
- Kept normal review navigation first.
- Moved challenge export to the Review Complete action area.
- Escape collapses the Challenge This Answer details and returns focus to its summary.


V1.4.8 Update:
- Moved Challenge This Answer after review navigation in tab order.
- Challenge remains collapsed and optional.
- Escape from Challenge now returns focus to the review navigation button.
- Hid Challenge panel outside active review states.


V1.4.12 Update:
- Rolled Challenge workflow back to a stable placeholder.
- Removed broken challenge form fields, counters, save flow, and export flow from the active review workflow.
- Preserved stable missed-question review navigation.
- Added recent-question avoidance for better variety.


V1.4.14 Update:
- Replaced details/summary Challenge experiment with a controlled dialog-style Challenge panel.
- Challenge This Answer opens a separate form with Proposed answer, Reasoning, Save Challenge, and Cancel Challenge.
- Escape closes the Challenge dialog and returns focus to Challenge This Answer.
- Review navigation remains stable outside the dialog.


V1.4.17 Update:
- Rebuilt from V1.4.14 modal base.
- Repaired Challenge button activation with direct click and keydown handlers.
- Added unique Challenge Review question titles.
- Added validation error message and focus to the first error field.
- Save, Cancel, and Escape close the modal and return focus to the review navigation action.
- Removed the A shortcut from instructions and spoken question text because it was unreliable with screen reader focus behavior.


V1.4.18 Update:
- Final polish for Challenge modal.
- Focus now lands on the unique Challenge Review heading first to reduce duplicate field announcements.
- Save and Cancel messages are shorter.
- Validation clears when the learner types in either Challenge field.
- Save, Cancel, and Escape continue to return focus to Next Missed Question or Finish Review.


V1.4.19 Update:
- Added a modalOpen state guard for the Challenge modal.
- Captures keydown events while the modal is open so underlying app shortcuts cannot run.
- Blocks background shortcuts until focus is inside the modal.
- Keeps Tab and Shift+Tab trapped inside the modal.
- Escape cancels the modal from anywhere while it is open.
- Added aria-describedby on the Challenge dialog for better modal context.


V1.4.20 Update:
- Added true modal keyboard capture for the Challenge modal.
- Blocks all background app shortcuts while the Challenge modal is open.
- Allows typing only inside modal edit fields.
- Keeps focus inside the modal with a focusin safety net.
- Moves focus into the modal synchronously when it opens to prevent early key leakage.


V1.4.21 Update:
- Fixed Challenge modal Save and Cancel buttons after modal keyboard guard.
- Space and Enter on modal buttons now manually activate the focused button.
- Modal still blocks all background shortcuts while open.
- Added Spacebar key compatibility for Challenge This Answer activation.


V1.4.28 Update:
- Rebased on V1.4.21 because that modal flow was the known-good baseline.
- Preserved V1.4.21 Challenge modal announcement, field labels, focus behavior, validation, Save, Cancel, and Escape behavior.
- Added persistent saved challenge queue, full export, pending count, and Clear Saved Challenges.
- Cleaned Review Complete to avoid stale review content and repeated review controls.

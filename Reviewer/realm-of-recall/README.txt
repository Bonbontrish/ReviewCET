REALM OF RECALL - REVIEWER GAME  (START HERE)

HOW TO RUN
1. Extract the realm-of-recall folder (keep the folders together).
2. Double-click index.html (Chrome, Edge, Firefox, Opera).
3. START QUEST > pick a category > read the notes (or STUDY SHEET) > BEGIN BATTLE.

WHAT'S NEW
- EDIT QUESTIONS (main menu): add, edit, copy, delete questions; paste many at once;
  edit categories (name, icon, enemy, colour, study notes); settings; backup/restore.
- 120 seconds per question (change it under SETTINGS).
- Categories: English / Language, Mathematics, Science, Abstract Reasoning, General Information.
- FINAL BOSS: mixes questions from every category. Locked until level 5 (change in SETTINGS).
  You have 5 hearts; lose them all and the boss wins.
- Everything reshuffles each game: question order, answer order, matching rows, true/false order.
  Questions you haven't seen or often miss are picked more often.
  "None of the above" / "No error" stay last. Picture questions keep A-B-C-D (letters are in the picture).
- SCOREBOARD: total score (all XP), level, coins, accuracy, best streak, mastery per category, recent battles.
- Bonus XP for fast answers and winning streaks. Sound effects (toggle with the speaker button).
- Keyboard: 1-5 pick an answer, Enter submits / continues.

IMPORTANT: WHERE YOUR EDITS ARE SAVED
Edits and progress live in this browser (localStorage). Clearing browser data erases them,
and another browser or computer starts fresh. Use EDIT QUESTIONS > EXPORT BACKUP regularly,
and LOAD BACKUP to bring it back.

FOLDER
index.html                  page structure + one <script> line per question file
css/style.css               pixel styling
img/abstract/               the 25 Abstract Reasoning pictures (cropped from your PDF)
js/util.js                  helpers + sound
js/stages.js                question helpers: mc(), tf(), ident(), match(), imgq()
js/categories.js            the starting categories + study notes
js/questions/*.js           starting questions (copied into the editor on first run)
js/bank.js                  the editable question bank (saving, backup, validation)
js/main.js                  game engine
js/editor.js                the in-game editor

ADD A NEW QUESTION FILE (optional, for big batches)
1. Copy js/questions/_template.js, set category: "english" | "math" | "science" | "abstract" | "general".
2. Add <script src="js/questions/your-file.js"></script> in index.html above js/bank.js.
New files are imported automatically the next time you open the game. Files already imported
are not re-imported, so edit existing questions in the in-game editor.
(RESTORE BUILT-IN in the editor re-adds any built-in questions you deleted.)

PASTE MANY FORMAT (EDIT QUESTIONS > PASTE MANY)
1. What is 6 x 7?
A. 36
B. 42
Answer: B
Explanation: 6 x 7 = 42.
Hint: Think 6 x 6, plus 6.

(blank line between questions; "Answer: True" makes True/False; no options makes a typed answer)

QUESTIONS I HAD TO SKIP OR ADJUST (the PDFs had no answer key / missing figures)
Mock Exam Math: skipped #17 (needs figure), #21 and #29 (choices don't match the problem);
  reworded #19 ("either line") and #27 ("halfway between x and b").
Mock Exam Science: skipped #15, #23, #27, #30, #33 (ambiguous, missing info, or no correct choice).
  #6 now says "hormone"; #11 rewritten so "Both a and b" doesn't depend on letters.
Mock Exam Language: skipped #2, #28, #30, #33, #35 (ambiguous). Underline items #16-20 rebuilt as
  "which part is incorrect?". #21 and #29 had small typos fixed.
All answers for the Mock Exam were worked out by me: please double-check them, and edit any you disagree with.
Abstract Reasoning and ACET General Info answers come from the answer keys in your PDFs.

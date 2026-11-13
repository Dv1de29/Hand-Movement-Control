# Plan

## What we have now: 
A tauri executable that loads a single display screen with a camera that shows ur hand and moves the mouse. 
<img width="1327" height="704" alt="Screenshot 2026-11-13 at 18 38 48" src="https://github.com/user-attachments/assets/f1278694-64c3-4178-a530-970858cbd702" />

The sends the landmarks in the Rust side of the project where its processed and it acts based on the signs and ladmarks


## Features

1. **2D hand model for sign creation**
   - Create signs either from the camera or by dragging the joints of the model
     <img width="256" height="256" alt="peace_sign_landmarks" src="https://github.com/user-attachments/assets/bd87d7a4-d9d4-4e66-b319-5d9bd05876d9" />
   - Name each sign and later assign it to an action
   - Integrated difficulty indicator that rates how hard a sign is to make, based on how often its action is used

2. **Action and sign menu**
   - Lists all actions and their assigned signs
   - Layout similar to the CS:GO settings menu

3. **Adjustable parameters**
   - Settings for tremor, limited range of motion, and similar needs
      - MAYBE: Option to tune these automatically from the user's own movement

4. **Pause sign**
   - One sign that disables control entirely, so a relaxed or loose hand cannot keep controlling the computer

5. **Status mini-box**
   - Small window in the top-right corner, which can be dismissed or moved
   - Shows a 2D model of the last sign detected
   - Stays active while recording signs

## Possible additions

- Tutorial that teaches one feature at a time
- Accounts that store configurations
- Different actions per active application (browser, IDE, video player)

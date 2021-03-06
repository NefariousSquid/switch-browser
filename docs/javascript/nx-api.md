# NX api

`window.nx` exposes a small API for accessing various browser features -- but we aren't sure what most of them do just yet!

## API

### isKeyboardShown

**type:** bool

**use:** indicates whether or not the keyboard UI is active

### canHistoryBack

**type:** function

### endApplet

**type:** function

**use:** exits out of the browser applet

### openTimeoutDialog

**type:** function

**use:** Show a message for a short period of time

**example:**

```js
  nx.openTimeoutDialog("I'm a message!");
```

### open1ButtonDialog

**type:** function

**use:** Show a message, with a custom "OK" button

**example:**

```js
nx.open1ButtonDialog("I'm a message!", "OK!");
```

### open2ButtonDialog

**type:** function

**use:** Show a message, with custom "OK" and "Cancel" buttons

**example:**

```js
nx.open2ButtonDialog("I'm a message!", "Cancel", "OK!");
```

### playSystemSe

**type:** function

**use:** Play a system sound effect, possible values:

  * SeToggleBtnFocus
  * SeToggleBtnOn
  * SeToggleBtnOff
  * SeCheckboxFocus
  * SeCheckboxOn
  * SeCheckboxOff
  * SeRadioBtnFocus
  * SeRadioBtnOn
  * SeSelectCheck
  * SeSelectUncheck
  * SeBtnDecide
  * SeTouchUnfocus
  * SeBtnFocus
  * SeKeyError
  * SeDialogOpen
  * SeWebZoomOut
  * SeWebZoomIn
  * SeWebNaviFocus
  * SeWebPointerFocus
  * SeFooterFocus
  * SeFooterDecideBack
  * SeFooterDecideFinish
  * SeWebChangeCursorPointer
  * SeWebTouchFocus
  * SeWebLinkDecide
  * SeWebTextboxStartEdit
  * SeWebButtonDecide
  * SeWebRadioBtnOn
  * SeWebCheckboxUncheck
  * SeWebCheckboxCheck
  * SeWebMenuListOpen

### stopSystemSe

**type:** function

### footer

**type:** object

* setAssign

    **type:** function

* setDefaultAssign

    **type:** function

* unsetAssign

    **type:** function

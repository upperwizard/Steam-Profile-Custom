# Steam-Profile-Custom
Steam Profile Custom Guide

## 1. Set Image Dimensions

Set the image width to `1000` and height to `1`, then remove the `id` attributes from both elements.

```javascript
$J('#image_width').val(1000).attr('id',''),$J('#image_height').val(1).attr('id','');
```

## 2. Set the Title Value

Define `v_trim` as an identity function and set the title value to a newline followed by 126 tab characters.

```javascript
v_trim=_=>{return _},$J('#title').val(' \n'+Array.from(Array(126),_=>'\t').join(''));
```









## Steam Console Commands

Open the Steam console(win+r):

```text
steam://open/console
```

### 1. Clear a Specific Achievement

Clears a specific achievement for the specified game. Replace `ACHIEVEMENT_API_NAME` with the actual achievement API name.

```text
achievement_clear 632470 ACHIEVEMENT_API_NAME
```

### 2. Reset All Stats and Achievements

Resets all stats for the specified game and may also clear its achievements. This does not necessarily delete local save files.

```text
reset_all_stats 632470
```

### 3. Sync Local Data to Steam Cloud

Attempts to upload local data to Steam Cloud for the specified game.

```text
cloud_sync_up 632470
```
Delete the save files, then sync to Steam Cloud. Combined with the commands above, this can make your game a completely fresh start.

![VMenu](vmenu.png)
# VMenu a Full-Featured Altv Menu UI made with Javascript by Florian L&auml;mmlein
#### Creates an interactive webview based Menu.
#### The VMenu System has over 51+ Items in the acctual stable version witch you can use.
&nbsp;
&nbsp;
***
## VMenu Features
- Easy to use, super fast and smoth.
- Heritage Slider.
- Multiple Menus.
- Statics Panel.
- Color Picker.
- Color Panel.
- Input Field.
- Grid Panel.
- Check Box.
- Switch.
- And Much more!
&nbsp;
&nbsp;
***
## How to use
```js
// 1: Import the VMenu.
import * as VMenu from './js/VMenu.js';


// 2. Setup an VMenu.
const MainMenu = new VMenu.PlayerUI("VMenu", "Menu Example", "", "right", 50, 50, 340, "{#fa8f32}");

MainMenu.addItem(new VMenu.PSeperator("Vehicles"));
MainMenu.addItem(new VMenu.PSlider("Slider", "~b~Slider ~w~example ~r~with ~g~color~y~", 0, "", "", 20, VMenu.DISABLED));
MainMenu.addItem(new VMenu.PSeperator("Seperator"));
MainMenu.addItem(new VMenu.PNumberList("NumberList", "NumberList example", 0, "", "", 9));

// 3. Start the VMenu.
MainMenu.start();

// 4. Listen to the VMenu.
MainMenu.ItemSelect.on((e) => {
    console.log(e);
});
```
&nbsp;
&nbsp;
***
## How to install

&nbsp;
***
## All Settings in the VMenu System
| <strong style="color: #6ba0ff;">Item</strong> | <strong style="color: #6ba0ff;">Description</strong> |
| --- | --- |
| `Menus` | |
| `PlayerUI` | |
| `SettingsUI` | |
| `GameUI` | |
| | |
| `Items PlayerUI` | |
| `PSubMenu` | |
| `PItem` | |
| `PSeperator` | |
| `PItemList` | |
| `PNumberList` | |
| `PCheckBox` | |
| `PSwitch` | |
| `PSlider` | |
| `PHeritageSlider` | |
| `PPercentageBar` | |
| `PImageItem` | |
| `PImageView` | |
| `PInput` | |
| `PColorPicker` | |
| `PStaticsPanel` | |
| `PColorPanel` | |
| `PGridPanel` | |
| | |
| `Items SettingsUI` | |
| `STab`  | |
| `STabData`  | |
| `SItem`  | |
| `SSeperator`  | |
| `SItemList`  | |
| `SNumberList`  | |
| `SCheckBox`  | |
| `SSwitch`  | |
| `SSlider`  | |
| `SPercentageBar`  | |
| `SImageItem`  | |
| | |
| `Items GameUI` | |
| `GSettings` | |
| `GPlayers` | |
| `GDetails` | |
| `GItem` | |
| `GSeperator` | |
| `GItemList` | |
| `GNumberList` | |
| `GCheckBox` | |
| `GSwitch` | |
| `GSlider` | |
| `GPercentageBar` | |
| `GPlayer` | |
| `GDetail` | |
| | |
| `Others` | |
| `Badge` | |
| `InstrutionalBar` | |
| `IButton` | |
| `IText` | |
| `MessageSmall` | |
| `MessageMidi` | |
| `MessageBig` | |
| `Color` | |

&nbsp;
&nbsp;
## Details about the Items
| <strong style="color: #6ba0ff;">Item</strong> | <strong style="color: #6ba0ff;">Attribute</strong> | <strong style="color: #6ba0ff;">Description</strong> | <strong style="color: #6ba0ff;">Type</strong> | <strong style="color: #6ba0ff;">Default value</strong> |
| --- | --- | --- | --- | --- |
| `PlayerUI` | | | | |
| | title | Menu title | String | None |
| | desc | Menu description | String | None |
| | font | Menu font style (Fantasy, Menus, ChaletLondon) | String | Fantasy |
| | float | Menu Display Position (left, right) | String | left |
| | x | Menu X from top left corner | Int | 50 |
| | y | Menu y from left corner | Int | 50 |
| | width | Menu width (min: 300, max: 400) | Int | 340 |
| | color | Menu custom color (hex, altv) | String | None |
| | max_items | Menu maximum items (max: 18, min: 1) | Int | 12 |
| `PSubMenu` | title | Menu title | String | None |
| | desc | Menu description | String | None |
| | viewTitle | Main Menu title | String | None |
| | viewDesc | Main Menu description | String | None |
| | onSide | Open SubMenu on side (true, false) | Bool | false |
| `PItem` | title | Item title | String | None |
| | desc | Item description not displayed | String | None |
| | value | Item value not displayed | Any | None |
| | icon | Item icon from [Fontawesome](https://fontawesome.com/v5.15/icons?d=gallery&p=2&m=free) | String | None |
| | tag | Item tag for Eventhandling not displayed | String | None |
| | badge | Item Badge from `Badge` | Badge | None |
| | ...kwargs | Item Eventhandlers | String | None |
| `PSeperator` | title | Item title | String | None |
| | badge | Item Badge from `Badge` | Badge | None |
| `PItemList` | title | Item title | String | None |
| | desc | Item description not displayed | String | None |
| | value | Item value not displayed | Any | None |
| | icon | Item icon from [Fontawesome](https://fontawesome.com/v5.15/icons?d=gallery&p=2&m=free) | String | None |
| | tag | Item tag for Eventhandling not displayed | String | None |
| | items | Item value list | Array | [[], []] |
| | imageItem | Item control for `PImageItem` | PImageItem | None |
| | ...kwargs | Item Eventhandlers | String | None |
| `PNumberList` | title | Item title | String | None |
| | desc | Item description not displayed | String | None |
| | value | Item value not displayed | Int | None |
| | icon | Item icon from [Fontawesome](https://fontawesome.com/v5.15/icons?d=gallery&p=2&m=free) | String | None |
| | tag | Item tag for Eventhandling not displayed | String | None |
| | max | Item maximum Numbers | Int | 1 |
| | ...kwargs | Item Eventhandlers | String | None |
| `PCheckBox` | title | Item title | String | None |
| | desc | Item description not displayed | String | None |
| | value | Item value not displayed | Bool | false |
| | icon | Item icon from [Fontawesome](https://fontawesome.com/v5.15/icons?d=gallery&p=2&m=free) | String | None |
| | tag | Item tag for Eventhandling not displayed | String | None |
| | ...kwargs | Item Eventhandlers | String | None |
| `PSwitch` | title | Item title | String | None |
| | desc | Item description not displayed | String | None |
| | value | Item value not displayed | Bool | false |
| | icon | Item icon from [Fontawesome](https://fontawesome.com/v5.15/icons?d=gallery&p=2&m=free) | String | None |
| | tag | Item tag for Eventhandling not displayed | String | None |
| | ...kwargs | Item Eventhandlers | String | None |
| `PSlider` | title | Item title | String | None |
| | desc | Item description not displayed | String | None |
| | value | Item value not displayed | Int | None |
| | icon | Item icon from [Fontawesome](https://fontawesome.com/v5.15/icons?d=gallery&p=2&m=free) | String | None |
| | tag | Item tag for Eventhandling not displayed | String | None |
| | max | Item maximum Slider range | Int | 1 |
| | ...kwargs | Item Eventhandlers | String | None |
| `PHeritageSlider` | title | Item title | String | None |
| | desc | Item description not displayed | String | None |
| | value | Item value not displayed | Int | None |
| | icon | Item icon from [Fontawesome](https://fontawesome.com/v5.15/icons?d=gallery&p=2&m=free) | String | None |
| | tag | Item tag for Eventhandling not displayed | String | None |
| | ...kwargs | Item Eventhandlers | String | None |
| `PPercentageBar` | title | Item title | String | None |
| | desc | Item description not displayed | String | None |
| | value | Item value not displayed | Int | None |
| | icon | Item icon from [Fontawesome](https://fontawesome.com/v5.15/icons?d=gallery&p=2&m=free) | String | None |
| | tag | Item tag for Eventhandling not displayed | String | None |
| | max | Item maximum PercentageBar range | Int | 1 |
| | ...kwargs | Item Eventhandlers | String | None |
| `PImageItem` | src | Item src image to path | String | None |
| `PImageView` | title | Item title | String | None |
| | desc | Item description not displayed | String | None |
| | value | Item value not displayed | Int | None |
| | icon | Item icon from [Fontawesome](https://fontawesome.com/v5.15/icons?d=gallery&p=2&m=free) | String | None |
| | tag | Item tag for Eventhandling not displayed | String | None |
| | src | Item src image to path | String | None |
| | viewTitle | Main Menu title | String | None |
| | viewDesc | Main Menu description | String | None |
| | viewFooter | Main Menu footer title | String | None |
| | badge | Item Badge from `Badge` | Badge | None |
| | ...kwargs | Item Eventhandlers | String | None |
| `PInput` | title | Item title | String | None |
| | desc | Item description not displayed | String | None |
| | value | Item value not displayed | String | None |
| | icon | Item icon from [Fontawesome](https://fontawesome.com/v5.15/icons?d=gallery&p=2&m=free) | String | None |
| | tag | Item tag for Eventhandling not displayed | String | None |
| | max | Item maximum input | Int | 100 |
| | pattern | Item input pattern | String | None |
| | ...kwargs | Item Eventhandlers | String | None |
| `PColorPicker` | title | Item title | String | None |
| | desc | Item description not displayed | String | None |
| | value | Item value from `Color` | Color | None |
| | icon | Item icon from [Fontawesome](https://fontawesome.com/v5.15/icons?d=gallery&p=2&m=free) | String | None |
| | tag | Item tag for Eventhandling not displayed | String | None |
| | viewTitle | Main Menu title | String | None |
| | viewDesc | Main Menu description | String | None |
| | ...kwargs | Item Eventhandlers | String | None |
| `PStaticsPanel` | title | Item title | Array, String | [None] |
| | value | Item value | Array, String | [None] |
| | icon | Item icon from [Fontawesome](https://fontawesome.com/v5.15/icons?d=gallery&p=2&m=free) | Array,String | [None] |
| | tag | Item tag for Eventhandling not displayed | Array, String | [None] |
| | max | Item maximum Static range | Array, Int | [100] |
| `PColorPanel` | title | Item title | String | None |
| | value | Item value (hex) | string | None |
| | colors | Item colors list (hex) | Array, String | [None] |
| | tag | Item tag for Eventhandling not displayed | String | None |
| `PGridPanel` | title | Item title | String | None |
| | value | Item value (min: 0, max: 24) | Int | None |
| | icon | Item icon from [Fontawesome](https://fontawesome.com/v5.15/icons?d=gallery&p=2&m=free) | String | None |
| | tag | Item tag for Eventhandling not displayed | String | None |
| | | | | |
| `SettingsUI` | | | | |
| | title | Menu title | String | None |
| | font | Menu font style (Fantasy, Menus, ChaletLondon) | String | Fantasy |
| | color | Menu custom color (hex, altv) | String | None |
| | max_items | Menu maximum items (max: 12, min: 1) | Int | 6 |
| | max_tabs | Menu maximum tabs (max: 12, min: 1) | Int | 6 |
| `STab` | title | Item title | String | None |
| | icon | Item icon from [Fontawesome](https://fontawesome.com/v5.15/icons?d=gallery&p=2&m=free) | String | None |
| `STabData` | title | Item title | String | None |
| | icon | Item icon from [Fontawesome](https://fontawesome.com/v5.15/icons?d=gallery&p=2&m=free) | String | None |
| `SItem` | title | Item title | String | None |
| | desc | Item description not displayed | String | None |
| | value | Item value not displayed | Any | None |
| | icon | Item icon from [Fontawesome](https://fontawesome.com/v5.15/icons?d=gallery&p=2&m=free) | String | None |
| | tag | Item tag for Eventhandling not displayed | String | None |
| | badge | Item Badge from `Badge` | Badge | None |
| | ...kwargs | Item Eventhandlers | String | None |
| `SSeperator` | title | Item title | String | None |
| | badge | Item Badge from `Badge` | Badge | None |
| `SItemList` | title | Item title | String | None |
| | desc | Item description not displayed | String | None |
| | value | Item value not displayed | Any | None |
| | icon | Item icon from [Fontawesome](https://fontawesome.com/v5.15/icons?d=gallery&p=2&m=free) | String | None |
| | tag | Item tag for Eventhandling not displayed | String | None |
| | items | Item value list | Array | [[], []] |
| | imageItem | Item control for `SImageItem` | PImageItem | None |
| | ...kwargs | Item Eventhandlers | String | None |
| `SNumberList` | title | Item title | String | None |
| | desc | Item description not displayed | String | None |
| | value | Item value not displayed | Int | None |
| | icon | Item icon from [Fontawesome](https://fontawesome.com/v5.15/icons?d=gallery&p=2&m=free) | String | None |
| | tag | Item tag for Eventhandling not displayed | String | None |
| | max | Item maximum Numbers | Int | 1 |
| | ...kwargs | Item Eventhandlers | String | None |
| `SCheckBox` | title | Item title | String | None |
| | desc | Item description not displayed | String | None |
| | value | Item value not displayed | Bool | false |
| | icon | Item icon from [Fontawesome](https://fontawesome.com/v5.15/icons?d=gallery&p=2&m=free) | String | None |
| | tag | Item tag for Eventhandling not displayed | String | None |
| | ...kwargs | Item Eventhandlers | String | None |
| `SSwitch` | title | Item title | String | None |
| | desc | Item description not displayed | String | None |
| | value | Item value not displayed | Bool | false |
| | icon | Item icon from [Fontawesome](https://fontawesome.com/v5.15/icons?d=gallery&p=2&m=free) | String | None |
| | tag | Item tag for Eventhandling not displayed | String | None |
| | ...kwargs | Item Eventhandlers | String | None |
| `SSlider` | title | Item title | String | None |
| | desc | Item description not displayed | String | None |
| | value | Item value not displayed | Int | None |
| | icon | Item icon from [Fontawesome](https://fontawesome.com/v5.15/icons?d=gallery&p=2&m=free) | String | None |
| | tag | Item tag for Eventhandling not displayed | String | None |
| | max | Item maximum Slider range | Int | 1 |
| | ...kwargs | Item Eventhandlers | String | None |
| `SPercentageBar` | title | Item title | String | None |
| | desc | Item description not displayed | String | None |
| | value | Item value not displayed | Int | None |
| | icon | Item icon from [Fontawesome](https://fontawesome.com/v5.15/icons?d=gallery&p=2&m=free) | String | None |
| | tag | Item tag for Eventhandling not displayed | String | None |
| | max | Item maximum PercentageBar range | Int | 1 |
| | ...kwargs | Item Eventhandlers | String | None |
| `SImageItem` | src | Item src image to path | String | None |
| | | | | |
| `GameUI` | | | | |
| | title | Menu title | String | None |
| | desc | Menu description | String | None |
| | font | Menu font style (Fantasy, Menus, ChaletLondon) | String | Fantasy |
| | color | Menu custom color (hex, altv) | String | None |
| `GSettings` | max_items | Menu maximum items (max: 10, min: 1) | Int | 5 |
| `GPlayers` | min_items | Menu minimum items (min: 1) | Int | 1 |
| | max_items | Menu maximum items (max: 20) | Int | 10 |
| `GDetails` | img | Menu image src to path | String | None |
| | max_items | Menu maximum items (max: 6, min: 1) | Int | 3 |
| `GItem` | title | Item title | String | None |
| | desc | Item description not displayed | String | None |
| | value | Item value not displayed | Any | None |
| | icon | Item icon from [Fontawesome](https://fontawesome.com/v5.15/icons?d=gallery&p=2&m=free) | String | None |
| | tag | Item tag for Eventhandling not displayed | String | None |
| | badge | Item Badge from `Badge` | Badge | None |
| | ...kwargs | Item Eventhandlers | String | None |
| `GSeperator` | title | Item title | String | None |
| | badge | Item Badge from `Badge` | Badge | None |
| `GItemList` | title | Item title | String | None |
| | desc | Item description not displayed | String | None |
| | value | Item value not displayed | Any | None |
| | icon | Item icon from [Fontawesome](https://fontawesome.com/v5.15/icons?d=gallery&p=2&m=free) | String | None |
| | tag | Item tag for Eventhandling not displayed | String | None |
| | items | Item value list | Array | [[], []] |
| | imageItem | Item control for `SImageItem` | PImageItem | None |
| | ...kwargs | Item Eventhandlers | String | None |
| `GNumberList` | title | Item title | String | None |
| | desc | Item description not displayed | String | None |
| | value | Item value not displayed | Int | None |
| | icon | Item icon from [Fontawesome](https://fontawesome.com/v5.15/icons?d=gallery&p=2&m=free) | String | None |
| | tag | Item tag for Eventhandling not displayed | String | None |
| | max | Item maximum Numbers | Int | 1 |
| | ...kwargs | Item Eventhandlers | String | None |
| `GCheckBox` | title | Item title | String | None |
| | desc | Item description not displayed | String | None |
| | value | Item value not displayed | Bool | false |
| | icon | Item icon from [Fontawesome](https://fontawesome.com/v5.15/icons?d=gallery&p=2&m=free) | String | None |
| | tag | Item tag for Eventhandling not displayed | String | None |
| | ...kwargs | Item Eventhandlers | String | None |
| `GSwitch` | title | Item title | String | None |
| | desc | Item description not displayed | String | None |
| | value | Item value not displayed | Bool | false |
| | icon | Item icon from [Fontawesome](https://fontawesome.com/v5.15/icons?d=gallery&p=2&m=free) | String | None |
| | tag | Item tag for Eventhandling not displayed | String | None |
| | ...kwargs | Item Eventhandlers | String | None |
| `GSlider` | title | Item title | String | None |
| | desc | Item description not displayed | String | None |
| | value | Item value not displayed | Int | None |
| | icon | Item icon from [Fontawesome](https://fontawesome.com/v5.15/icons?d=gallery&p=2&m=free) | String | None |
| | tag | Item tag for Eventhandling not displayed | String | None |
| | max | Item maximum Slider range | Int | 1 |
| | ...kwargs | Item Eventhandlers | String | None |
| `GPercentageBar` | title | Item title | String | None |
| | desc | Item description not displayed | String | None |
| | value | Item value not displayed | Int | None |
| | icon | Item icon from [Fontawesome](https://fontawesome.com/v5.15/icons?d=gallery&p=2&m=free) | String | None |
| | tag | Item tag for Eventhandling not displayed | String | None |
| | max | Item maximum PercentageBar range | Int | 1 |
| | ...kwargs | Item Eventhandlers | String | None |
| `GPlayer` | title | Item title | String | None |
| | status | Player Status (`STATUS_HOST`, `STATUS_ENTER`, `STATUS_LEAVE`, `STATUS_READY`) | String | `STATUS_HOST` |
| | badge | Item Badge from `Badge` | Badge | None |
| `GDetail` | title | Item title | String | None |
| | value | Item value | Any | None |
| | icon | Item icon from [Fontawesome](https://fontawesome.com/v5.15/icons?d=gallery&p=2&m=free) | String | None |
| | badge | Item Badge from `Badge` | Badge | None |
| | | | | |

&nbsp;
&nbsp;
***
## Legacy versions
This version of the VMenu are the acctual stable version which is supported for feature updates.

## Do you have any Ideas, Changes or Bugs ?
Please let me know in the Comments, i will try to fix or add waht you found/want :D
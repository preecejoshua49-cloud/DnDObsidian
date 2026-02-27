---
NoteIcon: item
Rarity: 
Item-Type: 
Requires-Attunement: false
Attunement-Details: 
Cursed: false
Sentient: false
Charges: 
Recharge: 
Creator: 
Current-Owner: 
Location: 
Value: 
---

<% tp.file.title %>
<% await tp.file.move("DnD/3. Resources/Magical Items/" + tp.file.title) %>

<%*
const hasTitle = !tp.file.title.startsWith("NewMagicalItem");
let title;
if (!hasTitle) {
    title = await tp.system.prompt("Enter Magical Item Name");
    await tp.file.rename(title);
} else {
    title = tp.file.title;
}
_%>

> [!infobox]
> # `=this.file.name`
> ###### Item Information
> Type | Stat |
> ---|---|
> Rarity | `=this.Rarity` |
> Item Type | `=this["Item-Type"]` |
> Requires Attunement | `=this["Requires-Attunement"]` |
> Charges | `=this.Charges` |
> ###### Ownership
> Type | Stat |
> ---|---|
> Current Owner | `=this["Current-Owner"]` |
> Location | `=this.Location` |
> Value | `=this.Value` |

# `=this.file.name`
*`=this["Item-Type"]`, `=this.Rarity`*

---

## Description
<% tp.file.cursor() %>

Write the physical description of the item here.

---

## Magical Properties

Write the item's magical effects, abilities, and mechanics here.

---

## History & Lore

- Creator: `=this.Creator`
- Origin Location: `=this.Location`

---

## DM Notes

Hidden mechanics, scaling states, plot hooks, or curse details.
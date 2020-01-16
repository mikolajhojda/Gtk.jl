## Overview
A full width bar for presenting contextual actions

GtkActionBar is designed to present contextual actions. It is expected to be displayed below the content and expand horizontally to fill the area.

It allows placing children at the start or the end. In addition, it contains an internal centered box which is centered with respect to the full width of the box, even if the children at either side take up different amounts of space.


### Functions
gtk_action_bar_new () <br>
Creates a new GtkActionBar widget <br><br>

gtk_action_bar_pack_start () <br>
Adds child to action_bar, packed with reference to the start of the action_bar <br><br>

gtk_action_bar_pack_end () <br>
Adds child to action_bar, packed with reference to the end of the action_bar <br><br>

gtk_action_bar_get_center_widget () <br>
Retrieves the center bar widget of the bar.<br><br>

gtk_action_bar_set_center_widget () <br>
Sets the center widget for the GtkActionBar.<br><br>

### Child Properties
GtkPackType   -  pack-type   -   Read / Write<br>
gint  -   position  -	Read / Write

#### Types and Values
struct	GtkActionBar<br><br>

“pack-type”         -       GtkPackType<br>
A GtkPackType indicating whether the child is packed with reference to the start or end of the parent.<br>
Flags: Read / Write<br>
Default value: GTK_PACK_START<br><br>

“position”        -         gint<br>
The index of the child in the parent.<br>
Flags: Read / Write<br>
Allowed values: >= -1<br>
Default value: 0<br>

#### Object Hierarchy

    +- GObject
    .  +- GInitiallyUnowned
    .  .  +- GtkWidget
    .  .  .  +- GtkContainer
    .  .  .  .  +- GtkBin
    .  .  .  .  .  +- GtkActionBar
<!--
Copyright (c) 2020, 2020 IBM Corporation and others.

This program and the accompanying materials
are made available under the terms of the Eclipse Public License 2.0
which accompanies this distribution, and is available at
https://www.eclipse.org/legal/epl-2.0/

SPDX-License-Identifier: EPL-2.0
-->
### This repository contains a patch to `org.eclipse.swt.widgets.Tree` for eclipse 2019-12 on GTK.

The fix for [bug 552096](https://bugs.eclipse.org/bugs/show_bug.cgi?id=552096) isn't very user-friendly. Now it seems to scroll (to the middle) even if not necessary.

For example, open the git repositories view and expand the tree so there are more rows than will fit in the view. Scroll to the bottom and select a item near the top of the view. Notice that the selection is scrolled to the middle. It makes it easy to land in the context menu for the wrong item if you don't move the mouse to right-click after making a selection.

### Instructions

Load this project into eclipse 2019-12 and build it.

Update org.eclipse.swt.gtk.linux.x86_64_3.113.0.v20191204-0601.jar with Tree.class within the build directory. Enjoy.

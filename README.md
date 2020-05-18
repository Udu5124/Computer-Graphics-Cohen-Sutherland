# Computer-Graphics-Cohen-Sutherland
Computer Graphics : Demonstrate ability to clip lines using the Cohen-Sutherland Algorithm.

#----------------------------------------------------------------------
Purpose:

  * Demonstrate ability to clip lines using the Cohen-Sutherland
    algorithm.

  * Demonstrate ability to write some additional (simple) C code.

#----------------------------------------------------------------------
Background:

  * The Cohen-Sutherland algorithm is explained in the handout
    posted to Canvas in the Modules section.

  * The goal for this homework is to read lines (from a ".line"
    file) and clip them using the Cohen-Sutherland algorithm and
    the supplied view parameters (from a ".view" file).  The
    clipped lines are then printed (along with the canvas size) to
    create a viewable ".sdf" file.

  * Line files have the following format.  (The basic structure is
    the same as the SVFM file, just with different entries.)

    - Blank lines are to be ignored.  (A blank line has no
      characters at all or is just whitespace.)

    - Lines with '#' as the first non-whitespace character are
      comments and are to be ignored.

    - A line with an 'l' as the first non-whitespace character is
      a line line (ha!).  There will be four numbers following
      the 'l': the p1X, p1Y, p2X, p2Y coordinates of the two
      endpoints that define the line.  The 'l' and the coordinates
      will be separated by whitespace.  Example:

        l  237.4    123   8      96.1

      Notice that the coodinates may be either integer or floating
      point numbers.

    - If a line starts with any other non-whitespace character, it
      should be silently ignored.  ('silently' means you should
      not print an error message.  Just ignore it.)

  * View files are as described in the previous homework.

#----------------------------------------------------------------------

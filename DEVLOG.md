# Developer Log (DEVLOG.md)

Minimum **6 entries** required.

### Entry 1
**Issue Encountered:** I started the DFS function and didn't know what order to check things in
**Error Messages or Symptoms:**  The program would crash or not go through the maze
**Attempts Made:**  I tried to make small tests to check the bounds, walls, and visits
**Final Resolution:** I made the function with basic conditions so that the recursion could run safely

---

### Entry 2
**Issue Encountered:** Check the indices before running DFS
**Error Messages or Symptoms:** The program was crashing when it got to the edges of the maze
**Attempts Made:**  I added codes that made sure the parents were being assigned after checking the bounds
**Final Resolution:** Moving the checks before made sure the parents were set to an appropriate index

---

### Entry 3
**Issue Encountered:** Cleaned up the logic and made it more organized
**Error Messages or Symptoms:**  There was nothing wrong, but it makes it easier for me and others to follow my code
**Attempts Made:**  I rearranged the code segments multiple times to find the most logical order
**Final Resolution:** I first check the invalid ones, then mark the valid ones already visited, and then check the exits and neighbors

---

### Entry 4
**Issue Encountered:** The path that was printed wasn't always correct
**Error Messages or Symptoms:**  The output path wasn't always clear
**Attempts Made:**  I checked the parent values in the DFS function that were getting overwritten
**Final Resolution:** I added an if statement that will only set the parents if they are still untouched

---

### Entry 5
**Issue Encountered:** The DFS was not connected to main()
**Error Messages or Symptoms:**  The maze printed, but it didn't show the final path
**Attempts Made:**  I checked where the entrance and exit were and called DFS after the maze was set up
**Final Resolution:** I called DFS using the entrance and then printed the result

---

### Entry 6
**Issue Encountered:** Code worked for small mazes up to 5 5, but didn't work past that
**Error Messages or Symptoms:**  The program would print No path found! for 6 6 and above
**Attempts Made:**  I ran tests 1 1, 2 2, 3 3, and so on to see when it would stop finding a path
**Final Resolution:**  I confirmed that the program only works on a smaller scale when the code stops finding paths starting at 6 6

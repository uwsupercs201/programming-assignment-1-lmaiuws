# Programming Assignment 1

## Goal: Learn Standard I/O (Input/Output), numeric datatypes, and mathematical operations.

### NOTE: The speed of light is 299,792,458 m/s. (This is actually how the meter is officially defined nowadays!). We have not specifically discuss several mathematical operators. You may find the `Math` class useful for this assignment. You can find details in section 4.1 of our textbook or [here](https://docs.oracle.com/javase/8/docs/api/java/lang/Math.html)

## Part 1

You may have seen the famous equation 
$$E_0 = mc^2$$
from Einstein's special theory of relativity.

This equation gives the energy, $E_0$, of an object with mass $m$ when it is standing still relative to an observer,
where $c$ is the speed of light.

$E_0$ may be called the "rest energy" of the object.

However, if the object is moving with speed $v$ relative to the observer, then its energy is
$$E_v = \frac{mc^2}{\sqrt{1 - v^2 / c^2}}.$$

The difference between these two energy levels, $$E_t=E_v - E_0$$, is the *energy needed to impart speed v m/s to an object of mass m kilograms
starting from rest*. Energy is measured in Joules (J).

### Your Assignment:

Create a Java class called `Energy` which prompts the user to enter a rest mass and a speed,
and then computes and prints how much energy it would take to get that mass up to that speed. NOTE: This is asking you to compute $E_t$. Example:

```
Enter a rest mass (in kilograms): 10
Enter a speed (in m/s): 10
Total energy: 500 J
```

After your program is working, use comments to answer the following questions in the `Energy.java` file, or include a .txt file called `Part_1_answers` in your GitHub repo. 

(1) In old-time (nonrelativistic) physics, the formula for energy was
$$E_v = \frac{1}{2}mv^2.$$ Today, we consider this formula to be a good approximation to the true energy
for speeds that are small compared to the speed of light.
What does this formula predict the energy should be if the mass is 1 gram
and the speed is 1 meter per second (you do not need the program to compute this!)? Does your program Energy (from question 1(a)) agree with this number?

(2) What do you think should happen if you run your program and enter a speed greater than the speed of
light? Try it. What happened?

## Part 2

You may also have heard that it is impossible for any object to go faster than light. But what if, say, you fire a rocket that goes at $0.9c$ (90\% of the speed of light), and *from inside of that rocket* you launch another rocket that also goes at $0.9c$ in the same direction?

In everyday life, we'd want to say that the inner rocket moves at $1.8c$ relative to you, but this is greater than
the speed of light! But Einstein was a thoughtful person, and he would tell you that if
object \# 1 moves at speed $v_1$ relative to you, and object \# 2 moves at speed $v_2$ relative to object \# 1,
all in a straight line in the same direction, then the speed of object \# 2 relative to you is
$$v = \frac{v_1 + v_2}{1 + v_1v_2/c^2}.$$


### Your assignment:

Create a Java class called `VelocityAdd` which prompts the user to enter two velocities, $v_1$ and $v_2$,
as in our discussion above, and then tells the user how fast the second object is moving relative to the original observer (the "combined" speed). NOTE: This means you should use the relativistic version.

Example:

```
Enter the first speed (in m/s): 10
Enter the second speed (in m/s): 25
The speed of the second object relative to the observer is: 35 m/s.
```

Once your program is working, use comments to answer the following questions in the `VelocityAdd.java` file, or include a .txt file called `Part_2_answers` in your GitHub repo.

(1) In nonrelativistic physics, the formula for velocity addition was
$$v = v_1 + v_2,$$
as we hinted above.
This formula is still considered a good approximation when $v_1$ and $v_2$ are small compared to $c$.
What does this formula predict the combined speed should be if $v_1 = 3$ m/s and $v_2 = 5$ m/s (you do not need the program for this)?
Does your program VelocityAdd(from question 2(a)) agree with this result?

(2) Run your program with the input $v_1 = 0.9c$ and $v_2 = 0.9c$. (You need to figure out what $0.9c$ is first.)
What is the output? How can you interpret it?

## Submitting the Assignment

When you're done, you can upload your files to this Repo and commit the changes.

Click Add files at the top right of the Repo page.

There are two options:

A) Click "Add Files" to create new Java files in the repo manually. Create new files with name `Energy.java` and `VelocityAdd.java` You can re-type or copy paste your code into those files.

B) Click "Upload Files" to just upload the `.java` files you already created. Navigate to the src folder on your computer and upload `Energy.java` and `VelocityAdd.java`.

Once you've created the file you want, or uploaded them, navigate to the bottom of the Page and hit "Commit changes". Ensure "Commit directly to the main branch." is selected. You'll need to "Commit changes" once for each file you "Create" in GitHub, but can upload multiple files before a single Commit.



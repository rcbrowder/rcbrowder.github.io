# What they don't teach you on the internet
By: Chris Browder

### Purpose

I had decided I wanted to be a Web Developer long before I decided to enroll in the Awesome Inc. Bootcamp. I tinkered around in college with HTML and CSS. I learned UNIX commands and downloaded a slick text editor. I felt like I knew some stuff.

Then I graduated.

Like many other college grads I got hit with the ~Real World~ pretty quickly. I couldn't find a job in any kind of programming or development role, not even as an intern. I just didn't have the skills. So I took a job as a Project Manager at Epic Systems in Madison, WI. Approximately 13 months later I had ascertained that I hated my job and Wisconsin. (Both Epic and Wisconsin are fine places for many people! Just not for me.) So I quit. I was young(-ish). I had money saved up. I was ready to become a Web Dev.

I soon realized it's not easy to teach yourself a career. It's possible. There are a million resources online that offer guided coding lessons, video tutorials, online classes, and billion pages of documentation. But it's very difficult going that route so I enrolled in a bootcamp.

Before I enrolled I did a lot of research on whether it would be worth it. I'm 9 days in and it has been everything I hoped it would be. So to help others make the decision I'm going to highlight some things I've learned that the online classes and tutorials didn't help me with.

#### Using Git w/ a Team

I learned some git on my own pre-bootcamp. I knew the basic commands and the purpose of git. Learning online deprived me of one crucial aspect of git - in the real world you won't be working by yourself. Working with a team to develop and publish a project is integral to any technical career. You can't learn it by yourself. One of the very first things we did in camp was to look at the structure of an organized remote git repository.
 <img src='https://nvie.com/img/git-model@2x.png' alt='Git Branching Model'>
 Source: <a href = 'https://nvie.com/posts/a-successful-git-branching-model/Source'>Vincent Driessen</a>

 They don't teach you this on Codecademy.

 Then we engineered our own merge conflict. A merge conflict occurs when you try to merge your code into the project when someone else has also altered that code.

 > Git can often resolve differences between merged branches. Usually, the changes are on different lines, or even in different files, which makes the merge simple for computers to understand. However, sometimes there are competing changes that Git needs your help with to decide which changes to incorporate in the final merge. Often, merge conflicts happen when people make different changes to the same line of the same file, or when one person edits a file and another person deletes the same file. You must resolve the conflict before you can merge the branches.
  \- GitHub Help

Here's an example of what a merge conflict might look like.
```
$ git status
# On branch branch-b
# You have unmerged paths.
#   (fix conflicts and run "git commit")
#
# Unmerged paths:
#   (use "git add ..." to mark resolution)
#
# both modified:      styleguide.md
#
no changes added to commit (use "git add" and/or "git commit -a")
```

This means either you or the person(s) you are conflicting with must change your code. Git makes this easy by doing something interesting to your code to help identify the conflicts! Git places conflict markers to show how your code is different from the other party's. When you open the file in your text editor, you'll see your changes from the base branch after the line `<<<<<<<`. Then after your changes there will be a separator `=======` followed by the conflicting code. To signify the end another marker will be displayed with the branch name like so `>>>>>>>> branch-newFeature`. All together it looks like this:

```
I want to put
<<<<<<<
apples in the code.
=======
oranges in the code.
>>>>>>> branch-newFruit
```

You can then decide what code to keep, delete the rest, and merge the branch.

Merge conflicts will happen all the time when working with a team so getting comfortable with seeing and resolving them is important. This is difficult to learn just by reading without actually experiencing it.

### One of many

There are tons of tips, tricks, tools, methods, techniques, and technologies we've discussed so far in Bootcamp. I hope to keep this blog updated with them so you can see for yourself the value of a program like this. Check back soon.

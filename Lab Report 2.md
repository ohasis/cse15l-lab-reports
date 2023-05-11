# Lab Report 2
Hello, fellow CS 15L student! Welcome to lab report number two.

---

## Part 1

Below is my code of ``StringServer``, which creates a basic search engine for string queries.

![Image](StringServer.png)

Below is my entry upon adding entering the request ``add-message?s=Hello`` :

![Image](Hello.png)

- My code calls the methods ``getPath()`` and ``getQuery()`` to take in the given path, query, 
respectively.
- The relevant argument to ``getPath()`` is ``/add-message``. Two of its specific values
are ``http://localhost:4004``, which is the URI, and ``4004``, which is the port number. ``/add-message`` is its 
path, which is assessed as a ``String`` and compared in the if-statement in ``StringServer``.
- The relevant argument to ``getQuery()`` is ``?s=Hello``. Its specific value is ``Hello``, which is a ``String``
used to determine whether or not the body of the if-statement should be executed.
- One field changed after this request is processed is ``message``, which is appended to include ``Hello``:
the first query. Another field that is changed is the ``String[] array`` ``parameters``, which is a two element
array containing the result of splitting the URI at its equal sign.

Below is my entry upon adding entering the request ``add-message?s=How Are You`` :

![Image](HowAreYou.png)

- My code calls the methods ``getPath()`` and ``getQuery()`` to take in the given path, query, 
respectively.
- The relevant argument to ``getPath()`` is ``/add-message``. Two of its specific values
are ``http://localhost:4004``, which is the URI, and ``4004``, which is the port number. ``/add-message`` is its 
path, which is assessed as a ``String`` and compared in the if-statement in ``StringServer``.
- The relevant argument to ``getQuery()`` is ``?s=How are you``. Its specific value is ``How are you``, which is a ``String``
used to determine whether or not the body of the if-statement should be executed.
- A field changed after this request is processed is ``message``, which is appended to include ``How are you``
in addition to ``Hello``, which it already contains. Another field that is updated is the ``String[] array`` ``parameters``,
which is a two element array containing the result of splitting the URI at its equal sign.


## Part 2

``public class ArrayExamples {


## Part 3

1) I learned more about writing test cases and debugging code in this lab, specifically when it comes to determining the difference between a symptom and a bug. While a symptom is an inconsistency between test output and input, a bug refers to the specific error in a program.

2) I also learned that, when it comes to writing failure-inducing input, I should note that errors on a small scale will tend to cause the same errors on a large scale, which means that writing test cases need not involve arrays of any particularly large sizes.

**Thank you! You have determined what I have learned about writing server files, as well as debugging code!**

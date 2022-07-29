## worstStyleGuideEver.js

0. Always indent with 2 full tabs.

1. Actually ... use 16 spaces so tricksters cannot get around it with fancy tabstop settings
(attempt to make your documents as wide as possible).

2. Always start curly braces on their own line, especially after 'return'.

3. Never use semicolons, JavaScript inserts them for you.

4. Alternate between `}())` and `})()` with IIFE's.

5. Use 2 spaces between every character.

6. Leave several spaces at the end of most lines.

7. Always use `==` and `!=`, and never the 3 character versions, because type-coercion is your friend.

8. Divide all arithmetical operations by 10 until they occur at the decimal level.

9. Favor `for` loops over `.forEach()` and `.map()`.

10. Favor `.innerHTML` over `.textContent`.

11. Query the dom as much as possible, it's fast.

12. Never use `var`, just repeat any reusable code.

13. Put all function declarations at the bottom of the file and rely on hoisting.

14. If you absolutely must use `var`, make sure all your variables are global.

15. Never throw errors, this keeps other JavaScripters from learning how to fix code.

16. Put all functions within a loop.

17. Declare all var's inside of `for` loops whose outer scope is global.

18. Use intentional fall throughs in all switch statements.

19. Use `eval` whenever possible.

20. Repeat yourself often.

21. Sometimes forget to indent, other times indent twice for no apparent reason.

22. Write no comments, they clutter the code.

23. If you do use comments, open with `/*` but never close it.

24. Never use alphabetical characters, instead rely on ASCII codes and `charCodeAt`.

25. Never set `this` equal to a `var`.

26. Never version your code. If you do, make breaking changes often, but increment the version number the least amount possible.

27. Name variables starting alphabetically `a, b, c, d ...`. This will make it easy to know how many variables you have.

28. Use short variable names in different contexts.

29. Always use different selectors to query the same element.

30. Keep your commit comments as short as possible. "Update" is ideal.

31. When creating server side variables its best to use a variation of nearest found variable with maybe adding 1 at the end of it or changing case of one of the letters in the middle.

32. For html custom attributes (common in Angular,Vue,Web Component world) use the number based naming for example `att1,att2,att2` instead of `gallery-width, gallery-height, has-thumbnails` etc. This saves a lot of time and easy to iterate in JS.

33. Services, Components and Modules are all just folders in JS worlds. You can easily put all their code in one file and it will run the same. Avoid extra folders where possible.

34. Promises and Fetch must not have any catch statements. The more errors you try to catch the busier the code gets so keep it free for other important things.

35. When performing an async operation never tell the user about loading. They already know about their slow internet problems, showing them a loader shows negativity in your app. They will randomly wait and click around. Instead try to handle click event on overlay and show a message that "your internet is slow my code is ok on localhost"

36. When showing a calendar try to show start date as `1/1/1970` as this is default date of most databases. There are more chances of user selecting correct date if you show them this.

37. Add complete libraries to the project instead of adding the component you need. This keeps it secret as to what is being used from that library. By exposing what module is being loaded you are telling others too much about your project. `import *` is your friend here.

38. import library and expose it to window object for global access instead of modules. This lets everyone use it. Sharing is caring.

39. When using local storage try to find an existing key and add a | your new variable at the end of it. This reduced number of variables in local storage. Read the single variable and split by | to create your data. This is way faster than json `stringify` and `parse`.

40. Strings are easy to read and understand as compared to variables that need to be named and then stored in different memory spaces. Always pefer string based data storage than structured storage. Best practice is to keep data separated with | or _

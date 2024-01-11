* [[Node.js Core Modules]] are separate

![[Pasted image 20231011152558.png]]
> » Each separate file is treated as a module in Node.js. » The most common use of modules is to use code or functions across different modules. * require is used to import modules, JSON files, and local files. It is passed a relative path as a string. « In our case, we have imported both of our modules on line 1 and line 2 of the index.js file. » exports or module.exports - All the variables or functions that we want to be accessible in other modules have to be exported.

![[Pasted image 20231011152623.png]]
> » The exports variable is available within a module’s file-level scope. « Instead of writing module.exports.Something, we can write exports.Something. We are using this in our square.js file. » The module.exports object is created by the Module system. « if we override exports by assigning it to something, else such as exports = function(){}, then exports would no longer point to module.exports. This is because the reassignment breaks the reference between module.exports and exports
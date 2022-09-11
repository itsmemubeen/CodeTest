<h1>Digitaltolk - Code Test</h1>

<h4>My Thoughts On The Code: </h4>

Resources can be used to prevent overloading
Traits can be used
controllers action should be single

There Are Some Pros And Cons In This Code

<h4>Pros</h4>
<hr>
<ol>
    <li>Repository pattern is used , which is best for managing code</li>
    <li>Variable Names are proper which makes code easy to understand</li>
    <li>Function Names are proper which makes code easy to understand</li>
<ol>
<h4>Cons</h4>
<ol>
    <li>Unnecessary Variables (like return $user = UserMeta::where('user_id', $user_id)->first()->$key; ) No need of $user here.</li>
    <li>Unreachable codes (like code after return statements).</li>
    <li>If conditions not properly structured. (like in function willExpireAt).</li>
    <li>Laravel Functions are not utilize.</li>
    <li>In code base repository class in defined by not utilized properly, like validations methods are not in use in this code.</li>
    <li>Few methods are too long . which can be trimed.</li>
</ol>

<h4>What I think can be improved</h4>
<ol>
    <li>There are a lot of if…else whose purpose is to only assign values to variables. I prefer using ternary operator if it’s just a simple variable assignment as it’s easier to read and cleaner.</li>
    <li>There are some conditional statements way below the functions that could result to returning values and therefore terminating the function. I prefer to put them higher up inside the function so that we don’t have to execute actions (variable assignments, other conditions, function calls, etc.) that would become useless if the said condition is satisfied.</li>
    <li>Excess empty lines after opening braces ({) and/or before closing braces (}) of functions.</li>
    <li>If there several chained functions, I prefer to put each on their own new line instead of in one line altogether as it presents a better glimpse of the code.</li>
    <li>It's just a minor observation, but there's an inconsistency on using the keywords else if and elseif.</li>
<ol>

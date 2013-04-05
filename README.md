CSS

Class names, use hypen, camelCase etc or more structured? ref1 BEM Independent CSS
grid-cell, gridCell ...


Class names, content-derived, content-independent or mixture of two? 
html5boilerplate seem to use a mixture. ref


avoidance of type selectors in favour of classes. ref
type selectors are:
    h1 { font-family: sans-serif }
    a { padding:1em }


Following on from using less type selectors, doing less of: ref

    .uilist { /* styles */ }
    .uilist a { /* styles */ }

    <nav class="uilist">
        <a href="#">Home</a>
        <a href="#">About</a>
        <a class="btn" href="#">Login</a>
    </nav>

And do more of:
    .uilist { /* styles */ }
    .uilist-item { /* styles */ }

    <nav class="uilist">
        <a class="uilist-item" href="#">Home</a>
        <a class="uilist-item" href="#">About</a>
        <span class="uilist-item">
            <a class="btn" href="#">Login</a>
        </span>
    </nav>



start using Javascript hook classes? ref
    <a href="/login" class="btn btn-primary js-login"></a>
As seen in Twitter.


preference for “single-class” pattern or “multi-class” pattern? ref

single-class
    .btn, .btn-primary { /* button template styles */ }
    .btn-primary { /* styles specific to save button */ }

    <button class="btn">Default</button>
    <button class="btn-primary">Login</button>


Multi-class
    .btn { /* button template styles */ }
    .btn-primary { /* styles specific to primary button */ }

     <button class="btn">Default</button>
     <button class="btn btn-primary">Login</button>


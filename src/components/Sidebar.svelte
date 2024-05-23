<script>
   let navItems = [];
</script>

<nav>
<ul>
 {#each navItems as item}
 <li><a href={item.href}>{item.text}</a></li>
 {/each}
 </ul>
</nav>


<aside>
    <ul>
        <li><a href="#">Link 1</a></li>
        <li><a href="#">Link 2</a></li>
        <li><a href="#">Link 3</a></li>
    </ul>
</aside>

<style>
    aside {
        background-color: #f4f4f4;
        padding: 10px;
        width: 200px;
        position: fixed;
        top: 0;
        left: 0;
        height: 100%;
    }

    ul {
        list-style-type: none;
        padding: 0;
        margin: 0;
    }

    li {
        list-style: none;
    }

    a {
        text-decoration: none;
        color: black;
    }

    a:hover {
        color: rebeccapurple;
    }
</style>

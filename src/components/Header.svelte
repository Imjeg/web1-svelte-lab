<script>
  export let navItems;
 </script>

 <header>
     <h1>This is my header</h1>
     <nav>
       <ul>
         {#each navItems as Item}
           <li><a href={Item.href}>{Item.text}</a></li>
         {/each}
       </ul>
     </nav>
 </header>

 <style>
   header{
     background: rebeccapurple;
     grid-column: 1 / 3;
   }
 </style>
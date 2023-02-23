<script lang="ts">
    import Menu from '../Menu/Menu.svelte'
    // import Bars from '/src/assets/icons/bars.svelte'
    // import MagnifyingGlass from '/src/assets/icons/magnifying-glass.svelte'

</script>

<header class="">
        <div class="flex flex-row justify-between items-center p-4">
        <img src="/src/assets/HT-logo-mobile-nav.svg" alt="HathiTrust logo">
        <div class="flex flex-row items-center p-0 gap-6">
            <svg id="Layer_2" data-name="Layer 2" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 10.5 9"> <g id="Layer_1-2" data-name="Layer 1"> <path d="m0,.75c0-.42.33-.75.75-.75h9c.42,0,.75.33.75.75s-.33.75-.75.75H.75c-.42,0-.75-.33-.75-.75Zm0,3.75c0-.42.33-.75.75-.75h9c.42,0,.75.33.75.75s-.33.75-.75.75H.75c-.42,0-.75-.33-.75-.75Zm10.5,3.75c0,.42-.33.75-.75.75H.75c-.42,0-.75-.33-.75-.75s.33-.75.75-.75h9c.42,0,.75.33.75.75Z"/> </g> </svg>
            <svg id="Layer_2" data-name="Layer 2" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 12 12"> <g id="Layer_1-2" data-name="Layer 1"> <path d="m9.75,4.88c0,1.08-.35,2.07-.94,2.88l2.97,2.97c.29.29.29.77,0,1.06s-.77.29-1.06,0l-2.97-2.97c-.81.59-1.8.94-2.88.94C2.18,9.75,0,7.57,0,4.88S2.18,0,4.88,0s4.88,2.18,4.88,4.88Zm-4.88,3.38c1.86,0,3.38-1.51,3.38-3.38s-1.51-3.38-3.38-3.38-3.38,1.51-3.38,3.38,1.51,3.38,3.38,3.38Z"/> </g> </svg>
        </div> 
    </div>
        <Menu />
   

</header>

<style>
    svg {
        @apply text-ht-neutral-900 m-auto h-4;
    }
</style>
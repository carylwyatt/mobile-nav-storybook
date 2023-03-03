<script lang="ts">
    import menuData from '../../../assets/menuData.json';
    let dropdownActive = {about: false, collection: false, libraries: false, news: false};

</script>

<nav>
    <ul>
        <li class="flex flex-col">
            <button on:click={() => dropdownActive.about = !dropdownActive.about} on:keyup={() => dropdownActive.about = !dropdownActive.about} class="flex flex-row justify-between items-center w-full p-4 font-bold">
                <span>About </span>
                <svg class="h-1" id="Layer_2" data-name="Layer 2" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 7.5 4.5"> )<g id="Layer_1-2" data-name="Layer 1"> <path d="m3.22,4.28L.22,1.28C0,1.07-.06.75.06.47.18.19.45,0,.75,0h6c.3,0,.58.18.69.46s.05.6-.16.82l-3,3c-.29.29-.77.29-1.06,0h0Z"/> </g> </svg>
            </button>
            <div class="py-4 bg-ht-neutral-50 {dropdownActive.about ? 'block' : 'hidden'}">
                <ul class="px-4 pt-2 space-y-6">
                   {#each menuData.about as linkText}
                   <li>{linkText}</li>
                   {/each}
                </ul>
            </div>
        </li>
        <li class="flex flex-col">
            <button  on:click={() => dropdownActive.collection = !dropdownActive.collection} on:keyup={() => dropdownActive.collection = !dropdownActive.collection} class="flex flex-row justify-between items-center w-full p-4 font-bold">
                <span>The Collection</span>
                <svg class="h-1" id="Layer_2" data-name="Layer 2" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 7.5 4.5"> <g id="Layer_1-2" data-name="Layer 1"> <path d="m3.22,4.28L.22,1.28C0,1.07-.06.75.06.47.18.19.45,0,.75,0h6c.3,0,.58.18.69.46s.05.6-.16.82l-3,3c-.29.29-.77.29-1.06,0h0Z"/> </g> </svg>
            </button>
            <div class="py-4 bg-ht-neutral-50 {dropdownActive.collection ? 'block' : 'hidden'}">
                <ul class="px-4 pt-2 space-y-6">
                   {#each menuData.collection as linkText}
                   <li>{linkText}</li>
                   {/each}
                </ul>
            </div>
        </li>
        <li class="flex flex-col">
            <button  on:click={() => dropdownActive.libraries = !dropdownActive.libraries} on:keyup={() => dropdownActive.libraries = !dropdownActive.libraries} class="flex flex-row justify-between items-center w-full p-4 font-bold">
                <span>Member Libraries</span>
                <svg class="h-1" id="Layer_2" data-name="Layer 2" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 7.5 4.5"> <g id="Layer_1-2" data-name="Layer 1"> <path d="m3.22,4.28L.22,1.28C0,1.07-.06.75.06.47.18.19.45,0,.75,0h6c.3,0,.58.18.69.46s.05.6-.16.82l-3,3c-.29.29-.77.29-1.06,0h0Z"/> </g> </svg>
            </button>
            <div class="py-4 bg-ht-neutral-50 {dropdownActive.libraries ? 'block' : 'hidden'}">
                <ul class="px-4 pt-2 space-y-6">
                   {#each menuData.memberLibraries as linkText}
                   <li>{linkText}</li>
                   {/each}
                </ul>
            </div>
        </li>
        <li class="flex flex-col">
             <div class="flex flex-row justify-between items-center w-full p-4 font-bold">
                <span>Join</span>
            </div>
        </li>
       <li class="flex flex-col">
            <button  on:click={() => dropdownActive.news = !dropdownActive.news} on:keyup={() => dropdownActive.news = !dropdownActive.news} class="flex flex-row justify-between items-center w-full p-4 font-bold">
                <span>News &amp; Events</span>
                <svg class="h-1" id="Layer_2" data-name="Layer 2" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 7.5 4.5"> <g id="Layer_1-2" data-name="Layer 1"> <path d="m3.22,4.28L.22,1.28C0,1.07-.06.75.06.47.18.19.45,0,.75,0h6c.3,0,.58.18.69.46s.05.6-.16.82l-3,3c-.29.29-.77.29-1.06,0h0Z"/> </g> </svg>
            </button>
            <div class="py-4 bg-ht-neutral-50 {dropdownActive.news ? 'block' : 'hidden'}">
                <ul class="px-4 pt-2 space-y-6">
                   {#each menuData.newsEvents as linkText}
                   <li>{linkText}</li>
                   {/each}
                </ul>
            </div>
        </li>
        <li class="flex flex-col bg-ht-neutral-50 border-t border-ht-neutral-200">
            <div class="flex flex-row justify-between items-center w-full p-4 font-bold">
                <span class="uppercase font-extrabold">Get Help</span>
                <svg class="h-3.5 fill-ht-primary-500" id="Layer_2" data-name="Layer 2" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 10.5 10.5"> <g id="Layer_1-2" data-name="Layer 1"> <path d="m9,0c.83,0,1.5.67,1.5,1.5v7.5c0,.83-.67,1.5-1.5,1.5H1.5c-.83,0-1.5-.67-1.5-1.5V1.5C0,.67.67,0,1.5,0h7.5ZM3.75,2.62c-.31,0-.56.25-.56.56s.25.56.56.56h2.21l-3.17,3.16c-.22.22-.22.58,0,.79.22.22.58.22.79,0l3.16-3.16v2.39c0,.31.25.56.56.56s.56-.25.56-.56v-3.75c0-.31-.25-.56-.56-.56h-3.56Z"/> </g> </svg>
            </div>
        </li>
        <li class="flex flex-col bg-ht-neutral-50 border-y border-ht-neutral-200 rounded-b-lg">
            <div class="flex flex-row justify-between items-center w-full p-4 font-bold">
                <span class="uppercase font-extrabold">Log In</span>
                <svg class="h-3.5 fill-ht-primary-500" id="Layer_2" data-name="Layer 2" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 10.5 12"> <g id="Layer_1-2" data-name="Layer 1"> <path d="m6.32,7.12c2.31,0,4.18,1.87,4.18,4.18,0,.38-.31.7-.7.7H.7c-.38,0-.7-.31-.7-.7,0-2.31,1.87-4.18,4.18-4.18h2.14ZM2.25,3c0-1.66,1.34-3,3-3s3,1.34,3,3-1.34,3-3,3-3-1.34-3-3Z"/> </g> </svg>
            </div>
        </li>
    </ul>
</nav>

<style> 
    nav ul li {
        font-size: 14px;
        line-height: 18px;
        letter-spacing: -0.01em;
    }
   
</style>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<script lang="ts">

  import * as Menubar from "$lib/components/ui/menubar";
  import Button1 from './button.svelte';
  import Icon1 from "$lib/images/duggup.png"
  import Icon2 from "$lib/images/image.png"
  import Icon3 from "$lib/images/explore.png"
  import Icon4 from "$lib/images/home.png"
  import Icon5 from "$lib/images/learn.png"
  import Icon6 from "$lib/images/post.png"
  import Icon7 from "$lib/images/img1.png"
  import Icon8 from "$lib/images/img2.png"
  import Icon9 from "$lib/images/img3.png"
  import Icon10 from "$lib/images/img4.png"
  import Icon11 from "$lib/images/img5.png"
  import Icon12 from "$lib/images/img6.png"
  import Icon13 from "$lib/images/betterup.jpg"
  import arrow from "$lib/images/arrow.png"
  import website from "$lib/images/website.png"
  import { Button } from "$lib/components/ui/button/index.js";
  function changeText() {
    var button = document.getElementById("myButton");
    if (button.textContent === 'Click Me') {
        button.textContent = 'Clicked';
    } else {
        button.textContent = 'Click Me';
    }
}
</script>
<style>
    .vertical_dotted_line {
        position: relative;
        left: 30%;
        border-left: 1px dotted gray;
        height: 240px;
        padding-left: 20px; /* Adjust as needed */
    }

    .circle {
        position: absolute;
        top: 50%;
        left: 0%;
        transform: translate(-50%, -50%);
        width: 20px; /* Adjust size as needed */
        height: 20px; /* Adjust size as needed */
        border: 2px solid blue;
        border-radius: 50%;
        background-color: white; /* Optional, adjust as needed */
    }
</style>

<body bg-fafafa>

<div class="pl-10 pr-10"> 
    <Menubar.Root class="flex justify-between items-center p-0  w-1424 h-73 border-b border-dotted border-black border-t-0 border-l-0 border-r-0 rounded-none">
        
        <Menubar.Root class="pr-0 border-0">
            <Menubar.Menu class=" pl-0">
                <Menubar.Item class="pl-0">
                    <img src={Icon1} class="p-0 h-6 w-6 ">
                </Menubar.Item>
                <Menubar.Item class="pl-0">duggup</Menubar.Item>
            </Menubar.Menu>
        </Menubar.Root>
    
        <Menubar.Root class="pr-0 border-0 pt-4 pb-4">
            <Menubar.Menu class="flex justify-end pr-0 pt-5 pb-5">
                <Menubar.Item class="pl-0">
                    <div class="rounded-md overflow-hidden">
                        <img src={Icon4} class="p-0 h-6 w-6">
                    </div>
                </Menubar.Item>
                <Menubar.Item >Home</Menubar.Item>
                <Menubar.Item class="pl-0">
                    <img src={Icon3}  class=" h-6 w-6 ">
                </Menubar.Item>
                <Menubar.Item >Explore</Menubar.Item>
                <Menubar.Item class="pl-0">
                    <img src={Icon5} alt="Home" class="p-0 h-6 w-6 ">
                </Menubar.Item>
                <Menubar.Item class="pr-5">Learn</Menubar.Item>
                <Menubar.Item class="pl-0 pr-10">
                    <Button variant="outline" class=" h-8 w-24 border-b-2 border-gray-700"><img src={Icon6} class="pr-3 pl-0 pb-0 pt-0 h-6 w-8 ">Post</Button>
                </Menubar.Item>
                <div class=" rounded-full overflow-hidden border-2 border-black">
                    <img src={Icon2} class="p-0 h-6 w-6">
                </div>
                <Menubar.Trigger>
                    Krishna Kiran
                    <svg xmlns="http://www.w3.org/2000/svg" class="pl-0 h-4 w-4 inline-block ml-1" viewBox="0 0 20 20" fill="currentColor">
                        <path fill-rule="evenodd" d="M10 12l5-5H5l5 5z" clip-rule="evenodd" />
                    </svg>
                </Menubar.Trigger>
                <Menubar.Content>
                    <Menubar.Item>Profile</Menubar.Item>
                </Menubar.Content>
            </Menubar.Menu>
        </Menubar.Root>
    </Menubar.Root>
</div>

<div class="pl-40 pt-10 flex flex-row">
    <div class="flex flex-col items-center">
        <div class="rounded-full overflow-hidden border-2 h-20 w-20">
            <img src={Icon2} class="p-0 h-20 w-20">
        </div>
        <p class="mt-2">Krishna</p>
        <p class="mt-2 ">Kiran</p>
    </div>

    <div class="flex flex-col  pl-10" style="width: 721px;">
        <p>Co-Founder and CEO at Duggup - Social network for people in tech. Ex-Amazon Head of Engineering. I write hot-takes on building a business, shipping delightful products and accelerating product and career growth.</p>
        <br>
        <Button1 />
    </div>

    <div class="flex flex-col pl-2 items-end" style="width: 410px; padding-right:200px;">
        <div class="rounded-full overflow-hidden">
            <img src={Icon1} class="p-0 h-6 w-6 rounded-full">
        </div>
        <p class="font-bold">Duggup</p>
        <p class="text-gray-500">Co-founder and CEO</p>
        <br>
        <div class="flex flex-row">
            <p>My Website</p>
            <div class="flex flex-col">
                <img src={website} class="pl-1 pr-1 h-6 w-6">
            </div>
            <div class="flex flex-row items-center">
                    <div class="h-3 w-3 border-4 border-gray-300 rounded-full mr-1"></div>
                    <div class="h-3 w-3 border-4 border-gray-300 rounded-full mr-1"></div>
                    <div class="h-3 w-3 border-4 border-gray-300 rounded-full" mr-6></div>
            </div>
        </div>
    </div>
</div>

<div class="pl-10 pt-10 pr-80 items-center">

    <div class="flex flex-row justify-end">
        <div class="flex flex-col  text-right">
            <p class="pt-20">Dec 2023</p>
        </div>
        <div class="flex flex-col pl-6 pr-4">
            <div class="vertical_dotted_line">
                <div class="circle"></div>
            </div>
        </div>
        <div class="flex flex-col  ">
            <div class="rounded-lg overflow-hidden">
                <img src={Icon7}  class="p-0 h-60 w-80 rounded-lg border border-gray-400">
            </div>
        </div>
        <div class="flex flex-col pl-10 pr-10">
            <div class="rounded-lg overflow-hidden">
                <img src={Icon8}  class="p-0 h-60 w-80 rounded-lg border border-gray-400">
            </div>
        </div>
    </div>

    <div class="flex flex-row justify-end">
        <div class="flex flex-col justify-end pt-10 pr-0">
            <div class="flex justify-end p-0">
                <div class="rounded-full overflow-hidden">
                    <img src={Icon1} class="p-0 h-10 w-10 rounded-full">
                </div>
            </div>
            <p class="font-bold text-right">Duggup</p>
            <p class="text-right text-xs">San Francisco Bay Area</p>
            <p class="text-right text-xs">Joined</p>
            <p class="text-right text-xs">Nov 2023</p>
        </div>
        <div class="flex flex-col pl-6 pr-4">
            <div>
                <img src={arrow} class="h-3 w-3">
            </div>
            <div class="vertical_dotted_line" style="height: 160px;">
                <div class="circle" style="border: 5px solid blue;"></div>
            </div>
        </div>
        <div class="flex flex-col">
            <div class="rounded-md overflow-hidden pt-10 pl-0 pr-10" style="width: 721px;">
                <img src={Icon9}  class="p-0 h-30 rounded-md border border-gray-400">
            </div>
        </div>
    </div>

    <div class="flex flex-row justify-end">
        <div class="flex flex-col text-right">
            <p class="pt-20">Dec 2023</p>
        </div>
        <div class="flex flex-col pl-6 pr-4">
            <div class="vertical_dotted_line">
                <div class="circle" ></div>
            </div>
        </div>
        <div class="flex flex-col">
            <div class="rounded-md overflow-hidden ">
                <img src={Icon10}  class="p-0 h-60 w-80 rounded-md border border-gray-400">
            </div>
        </div>
        <div class="flex flex-col">
            <div class="rounded-md overflow-hidden pl-10 pr-10">
                <img src={Icon11}  class="p-0 h-60 w-80 rounded-md border border-gray-400">
            </div>
        </div>
    </div>

    <div class="flex flex-row justify-end">
        <div class="flex flex-col justify-end pt-10 pr-0">
            <div class="flex justify-end">
                <div class="rounded-full overflow-hidden">
                    <img src={Icon13} class="p-0 h-10 w-10 rounded-full">
                </div>
            </div>
            <p class="font-bold text-right">BetterUp</p>
            <p class="text-right text-xs">San Francisco Bay Area</p>
            <p class="text-right text-xs">Joined</p>
            <p class="text-right text-xs">Sep 2022</p>
        </div>
        <div class="flex flex-col pl-6 pr-4">
            <div>
                <img src={arrow} class="h-3 w-3">
            </div>
            <div class="vertical_dotted_line" style="height: 160px;">
                <div class="circle" style="border: 5px solid blue;"></div>
            </div>
        </div>
        <div class="flex flex-col">
            <div class="rounded-md overflow-hidden pt-10 pl-0 pr-10 " style="width: 721px;">
                <img src={Icon12}  class="p-0 h-30 rounded-md border border-gray-400">
            </div>
        </div>
    </div>

</div>

</body>
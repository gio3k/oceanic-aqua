<link href="https://fonts.googleapis.com/icon?family=Material+Icons|Material+Icons+Outlined|Material+Symbols+Outlined"
      rel="stylesheet">

<script>
    let username = '';
</script>

<div class="relative flex flex-col flex-wrap justify-center items-center min-h-screen">
    <div class="absolute inset-0 opacity-30 dark:opacity-20 dark:invert bg-[length:140px_140px] bg-[url(/backgrounds/dot-seamless-pattern.svg)] bg-center"></div>

    <div class="flex flex-row flex-wrap">
        <div class="relative max-w-xs bg-white bg-opacity-80 p-6 m-3 ring-1 ring-gray-900/5 rounded-lg">
            <div class="flex flex-row justify-between items-center">
                <div class="flex flex-col">
                    <span class="text-4xl font-semibold">Gio</span>
                    <span class="text-gray-900 text-opacity-40">{username}</span>
                </div>
                <div class="relative">
                    <img src="picture.jpeg" class="ring-1 ring-gray-900/5 w-16 rounded-full" alt="Profile picture">
                </div>
            </div>
            <div class="pt-3">
                I'm an 18 year-old full-stack developer in Perth, Western Australia 💖
            </div>
            <div class="flex flex-col pt-4 space-y-2 text-gray-500">
                <a href="mailto:lotuspar0@gmail.com" on:mouseenter={()=>username = "lotuspar0@gmail.com"}>
                    <div class="p-3 rounded-sm border-gray-400 dark:border-gray-500 border-l-2 hover:border-l-4 hover:bg-gray-200 transition-all">
                        <span class="material-icons material-icons-outlined align-middle -mt-1">account_circle</span>
                        email me
                    </div>
                </a>
                <a href="https://github.com/lotuspar" on:mouseenter={()=>username = "@lotuspar"}>
                    <div class="p-3 rounded-sm border-gray-400 dark:border-gray-500 border-l-2 hover:border-l-4 hover:bg-gray-200 transition-all">
                        <span class="material-symbols material-symbols-outlined align-middle -mt-1">deployed_code_history</span>
                        find me on github
                    </div>
                </a>
            </div>
        </div>
    </div>
</div>
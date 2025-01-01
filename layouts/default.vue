<template>
    <div>
        <AppHeader />
        <main class="container min-h-[80%] p-4">
            <slot/>
        </main>
        
        <AppFooter>
            <div class="flex justify-end p-4">
                <p>we are use the default layout</p>
            </div>
        </AppFooter>
    </div>
</template>
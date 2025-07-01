<script lang="ts">
  import SearchBar from '$lib/SearchBar.svelte';
</script>

<nav style="background-color: #F0F0F0;" class="text-black">
    <div class="max-w-7xl mx-auto px-2 sm:px-4 lg:px-4">
        <div class="flex items-center justify-between h-20">
            <img src="/logo.png" alt="Logo" class="h-14" />
            <div class="ml-4 w-64">
                <SearchBar />
            </div>
            <div class="icon-group flex items-center space-x-4 ml-auto">
                <img src="/settings.png" alt="Settings" class="h-9" />
                <img src="/notifications.png" alt="Notifications" class="h-9" />
                <img src="/cart.png" alt="Cart" class="h-9" />
                <img src="/avatar.png" alt="Avatar" class="h-12" />
            </div>
        </div>
    </div>
</nav>

<style>
.icon-group img {
  cursor: pointer;
}
</style>

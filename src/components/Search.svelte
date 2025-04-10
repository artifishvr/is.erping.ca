<script>
    let input = "";

    function goToPage() {
        if (!input) return;
        window.location.href = "/" + input;
    }
</script>

<div class="flex mt-2 max-w-sm">
    <input
        type="text"
        placeholder="name"
        class="bg-zinc-900 text-white p-2 rounded-md rounded-r-none border-none"
        bind:value={input}
        onkeydown={(e) => e.key === "Enter" && goToPage()}
    />
    <button
        class="bg-zinc-800 text-white p-2 rounded-md rounded-l-none border-none cursor-pointer"
        onclick={goToPage}
    >
        check
    </button>
</div>

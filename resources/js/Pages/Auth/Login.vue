<template>
    <form action="">
        <div class="w-1/2 mx-auto">
            <div>
                <label for="email" class="label">E-mail (username)</label>
                <input type="text" id="email" class="input" />
                <div class="input-error">Potential Erros</div>
            </div>
            <div class="mt-4">
                <label for="password" class="label">Password</label>
                <input type="password" id="password" class="input" />
                <div class="input-error">Potential Erros</div>
            </div>
            <div class="mt-4">
                <button class="btn-primary w-full" type="submit">Login</button>
            </div>
        </div>
    </form>
</template>
<script setup></script>

<template>
<article>
    <div class="thrd-section">
        <header>
            <div class="title">
                <h1>ABOUT</h1>
            </div>
        </header>
        <main>
            <div class="text">
                <div class="para" v-bind:key="abt.id" v-for="abt in about">
                    {{abt.paragraph}}
                </div>
            </div>
            <div class="skill-sect">
                <div class="ss">

                    <ul>
                        <li>
                            <p>JAVASCRIPT</p>
                        </li>
                        <li>
                            <p>NODE.JS</p>
                        </li>
                        <li>
                            <p>PYTHON</p>
                        </li>
                    </ul>
                </div>
            </div>
        </main>
    </div>
</article>
</template>

<script>
export default {
    props: ["about"]
}
</script>
<style scoped>
article{
    padding: 0 10px;
    margin: 0 auto;
    max-width: var(--mw);
}
ul{
    padding: 0;
    margin: 0;
    display: block;
    margin: 20px 0;

}
li{
    background: #665e5e46;
    margin: 5px 0;
    padding: 3px 10px;
    
}
</style>
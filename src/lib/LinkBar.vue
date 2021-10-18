<template>
    <article>
        <ul class="bar">
      
           
            <li>
                <g-link>
                        <g-image alt="facebook link" src="/facebook.svg" width="60" />
                </g-link>
            </li>
            <li>
                <g-link>
                        <g-image alt="instagram link" src="/instagram.svg" width="60" />
                </g-link>
            </li>
            <li>
                <g-link>
                        <g-image alt="twitter link" src="/twitter.svg" width="60" />
                </g-link>
            </li>
        </ul>

    </article>
</template>
<script>
export default {
    name: "LinkBar"
}
</script>

<style scoped>
article{
    top:0;
    position: fixed ;
    padding: 10px;
    border: red solid 1px;
}
ul{
    border: blue solid 1px;
    display: flex;
    flex-direction: column;
    padding: 0;
    margin:0;
    

}

</style>
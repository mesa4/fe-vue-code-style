# fe-vue-code-style
базовые правила для написания общепонятного кода

### используем `PascaleCase` для именований компонентов

:x:
```vue
// bad
<script>
import cardBoard from 'cardBoard.vue'

export default {
    components: {
        cardBoard
    }
}
</script>
```

:white_check_mark:
```vue
// good
<script>
import CardBoard from 'cardBoard.vue'

export default {
    components: {
        CardBoard
    }
}
</script>
```

### компоненты в тэмплэйтах и скрипте

:x:
```vue
// bad
<template>
    <zalypa-bobra></zalypa-bobra>
</template>

<script>
import ZalypaBobra from 'ZalypaBobra.vue';

export default {
    components: {
        'zalypa-bobra': ZalypaBobra
    }
}
</script>
```

:white_check_mark:
```vue
// good
<template>
    <ZalypaBobra />
</template>

<script>
import ZalypaBobra from 'ZalypaBobra.vue';

export default {
    components: {
        ZalypaBobra
    }
}
</script>
```

###
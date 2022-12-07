# Custom Hooks

__Hooks__ personalizados de __Reac__ para reutilizar en otros proyectos

## Hooks
- [useForm](#useformsjs)

### useForms.js

Este __hook__ nos permite automatizar la creación de __controles de formulario__.
Para iniciar este _hook_ después de su importación, por ejemplo creando el _control de formulario_ "apellidos" escribimos;

```react
const {apellidos, handleInputChange, handleResetForm} = useForm({
    apellidos: 'González Tenreiro'
})
```

Luego en el componente de react podemos escribir:

```react
<input
    name='apellidos'
    value={apellidos}
    onChange={handleInputChange}
/>
```

Podemos tener un botón de reseteo de los campos:

```react
<button
    onClick={()=>handleResetForm()}
>Reiniciar</button>
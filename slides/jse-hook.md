##  Jse

De selectie van entities gaat via een hook en een callback.

```
function MODULE_jse_info() {
    return array(
        'projects' => array(
            'label' => t('Projects'),
            'callback' => 'example_get_jse_entity_ids',
        )
    );
}

function example_get_jse_entity_ids() {
    return array(
        'node' => array(1, 5, 56),
        'user' => array(23, 1)
    );
}
```
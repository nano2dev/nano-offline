![line](https://github.com/fwd/n2/raw/master/.github/line.png)

<h1 align="center">Nano.to Developer Tools (Beta)</h1>

![line](https://github.com/fwd/n2/raw/master/.github/line.png)

### One-time Charge

Accept non-custodial NANO payments on any website.

```html
<script src="https://dev.nano.to/pay.js"></script>

<script>
    nano.charge({ 
        amount: 0.1,
        address: 'YOUR_ADDRESS', 
        success: (block) => {
        	console.log(block)
        }
    })
</script>
```



### Pay Per View

Monetize any website element. 

```html
<script src="https://dev.nano.to/pay.js"></script>
<script>
    nano.ppv({ 
        element: '.premium', // all with class .premium
        amount: 0.1,
        address: 'YOUR_ADDRESS', 
        background: 'blue' 
        success: (block) => {
        	// Element(s) are automatically shown.
        	console.log(block)
        }
    })
</script>
```

### Nano.to eCommerce (Private Beta)

**Supported:**

- Printful
- WooCommerce
- Shopify

> Contact hello@nano.to for Beta access.

```html
<script src="https://dev.nano.to/pay.js"></script>

<script>
    nano.checkout({ 
    	order,
        amount: 0.1,
        address: 'YOUR_ADDRESS', 
        api_key: 'YOUR_PUBLIC_API_KEY',
        success: (block) => {
        	console.log(block)
        }
    })
</script>
```

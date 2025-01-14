<div align="center">
	<img src="https://logsnag.com/og-image.png" alt="LogSnag"/>
	<br>
    <h1>LogSnag</h1>
	<p>Get notifications and track your project events.</p>
	<a href="https://discord.gg/dY3pRxgWua"><img src="https://img.shields.io/discord/922560704454750245?color=%237289DA&label=Discord" alt="Discord"></a>
	<a href="https://docs.logsnag.com"><img src="https://img.shields.io/badge/Docs-LogSnag" alt="Documentation"></a>
	<br>
	<br>
</div>


## Installation

```sh
pip3 install logsnag
```

## Usage

### Import Library

```python
from logsnag import LogSnag
```

### Initialize Client

```python
logsnag = LogSnag(token='7f568d735724351757637b1dbf108e5', project="my-saas")
```

### Publish Event

```python
logsnag.publish(
    channel="waitlist",
    event="User Joined",
    description="Email: john@doe.com",
    icon="🎉",
    tags={
      "email": "john@doe.com",
      "user-id": "uid-12"  
    },
    notify=True
)
```

### Publish Insight

```python
logsnag.insight(
    title='User Count',
    value=100,
    icon='👨',
)
```

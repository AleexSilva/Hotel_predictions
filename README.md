# Fake Hotel

## Who Will Cancel?

*Fake Hotel* is preparing for the summer vacation season; however, they are concerned that many of their customers cancel at the last minute, leaving them with empty rooms. Some guests simply do not show up, and although a reservation fee is sometimes charged, the majority of profits come when guests pay the remainder upon checking in.

Using their data, they would like you to help identify customers who are more likely to cancel so they can follow up with them. If they do need to cancel, they hope it happens as early as possible.

## Data

*Fake Hotel* has two branches: one located in the state capital, "City Hotel," and another in a coastal community, "Resort Hotel."

The data they provided is in CSV format, where each row represents a reservation with the following attributes:

```python
import pandas as pd

data = pd.read_csv('hotel_bookings_training.csv')
```
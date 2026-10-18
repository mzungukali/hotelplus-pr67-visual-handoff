# Booking.com wizard entry, 18 October 2026

Local Distribution Central at `http://127.0.0.1:4188/distribution-central`, property Karura Canopy Hotel. The page is the branch UI. The Booking.com read was served as the contract from `BookingComConnectionService.read`, including the absent-connection response that matches preview application `2432c2448925d6c50c740d813387275669650aa9` (no connection row, provider configuration missing). Opening the wizard sent only GET. It did not create a connection or a channel property.

| File | Viewport | Result |
| --- | --- | --- |
| `absent-1440.png` | 1440×900 | Connection absent and provider configuration missing. Lookup and save disabled. |
| `absent-390.png` | 390×844 | Same |
| `channel-property-1440.png` | 1440×900 | Connection open, channel property missing. Lookup and save disabled. |
| `channel-property-390.png` | 390×844 | Same |
| `ready-1440.png` | 1440×900 | After the channel property is recorded. Lookup enabled. Save stays disabled until rooms are loaded. Booking.com is not activated. |
| `ready-390.png` | 390×844 | Same |
| `permission-1440.png` | 1440×900 | HTTP 401. Sign-in refusal. No retry. |
| `permission-390.png` | 390×844 | Same |
| `unavailable-1440.png` | 1440×900 | Upstream connection dropped. Retryable unavailable notice. |
| `unavailable-390.png` | 390×844 | Same |

`evidence.json` records the measured button state for each capture.

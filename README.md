# Medikit — 10‑Minute Medicine Delivery (Flutter Template)

This is a starter Flutter app designed for Android + iOS with a clean architecture and placeholder screens for:
- Login/Signup
- Homepage with search + prescription upload
- Cart & Checkout
- Orders & Live Order Tracking (map placeholder)
- Profile
- Basic services & state (Provider)

## Quick start
1) Install Flutter SDK and create a fresh project:
```bash
flutter create medikit
```
2) Replace the generated `lib/` and `pubspec.yaml` with the ones from this template.
3) Get packages and run:
```bash
flutter pub get
flutter run
```
4) (Optional) To enable maps & location:
   - Add your Google Maps API keys to Android and iOS (see comments in `order_tracking_screen.dart`).
   - Add required platform permissions (see below).

### Android permissions (AndroidManifest.xml)
- ACCESS_FINE_LOCATION
- ACCESS_COARSE_LOCATION
- INTERNET

### iOS permissions (Info.plist)
- NSLocationWhenInUseUsageDescription
- NSLocationAlwaysAndWhenInUseUsageDescription
- NSAppTransportSecurity -> NSAllowsArbitraryLoads (dev only; remove in prod)

## Next steps
- Connect Auth (Firebase Auth/OTP) in `services/auth_service.dart`
- Hook a real backend in `services/api_service.dart`
- Replace mock data with real inventory & orders
- Add Razorpay/PayU/Stripe in checkout
- Implement pharmacy license & prescription verification workflows

---
This template is MIT licensed. Use it freely for your Medikit build.

# Phoenix-express
Pin and Deliver
Phoenix Express Driver Mobile App
Enterprise-grade React Native driver application for the Phoenix Express delivery platform. Built with Expo for rapid development and deployment to iOS and Android.

Features
🚗 Delivery Management
	•	Real-time delivery assignment and acceptance
	•	Live GPS tracking with 1-second refresh rate
	•	Turn-by-turn navigation integration
	•	Delivery status updates (picked up, en route, delivered)
	•	Customer communication and notes

💰 Earnings & Payouts
	•	Real-time earnings tracking
	•	Daily/weekly/monthly earnings breakdown
	•	Instant payout requests to Chime account
	•	Referral bonus tracking ($100 per driver)
	•	Performance metrics and incentives

📍 Location Tracking
	•	Continuous background location tracking
	•	Geofencing with entry/exit detection
	•	Heat map visualization of active deliveries
	•	Predictive location forecasting
	•	Route optimization

👤 Driver Profile
	•	Complete profile management
	•	Vehicle information and verification
	•	Banking account setup
	•	Rating and review system
	•	Performance statistics

🔔 Notifications
	•	Push notifications for new deliveries
	•	Earnings alerts
	•	Delivery status updates
	•	System notifications

Installation
Prerequisites
	•	Node.js 16+ and npm/yarn
	•	Expo CLI: `npm install -g expo-cli`
	•	iOS: Xcode 14+ (for iOS builds)
	•	Android: Android Studio (for Android builds)

Setup
	1.	Install dependencies:


￼
	2.	Set up environment variables:
Create a `.env` file in the mobile directory:


￼
	3.	Start the development server:


￼
	4.	Run on iOS or Android:


￼
Project Structure

￼
Key Components
DriverApp Component
Main delivery management interface with:

	•	Available deliveries list
	•	Current delivery tracking
	•	Real-time location updates
	•	Status management

Authentication
	•	Secure token storage with Expo Secure Store
	•	JWT-based API authentication
	•	Auto-login on app launch
	•	Sign out functionality

Location Tracking
	•	Background location tracking
	•	5-second update interval during deliveries
	•	10-meter distance threshold
	•	Haversine distance calculations

Notifications
	•	Push notification setup
	•	Delivery alerts
	•	Earnings notifications
	•	Customizable sound and vibration

API Integration
Authentication Endpoints
	•	`POST /api/auth/login` - Driver login
	•	`POST /api/auth/register` - Driver registration
	•	`POST /api/auth/logout` - Driver logout

Delivery Endpoints
	•	`GET /api/deliveries/available` - Get available deliveries
	•	`POST /api/deliveries/{id}/accept` - Accept delivery
	•	`PUT /api/deliveries/{id}/status` - Update delivery status
	•	`POST /api/deliveries/{id}/location` - Update location

Driver Endpoints
	•	`GET /api/drivers/profile` - Get driver profile
	•	`PUT /api/drivers/profile` - Update profile
	•	`GET /api/drivers/earnings` - Get earnings data
	•	`POST /api/drivers/request-payout` - Request payout

Building for Production
iOS Build

￼
Android Build

￼
App Store & Google Play
	1.	Set up EAS account: `eas login`
	2.	Configure app.json with app details
	3.	Submit to stores using EAS Submit

Testing
Unit Tests

￼
Manual Testing Checklist
	•	Login/signup flow
	•	Delivery acceptance
	•	Location tracking accuracy
	•	Status updates
	•	Earnings calculation
	•	Payout requests
	•	Profile updates
	•	Notifications
	•	Offline functionality
	•	Background location tracking

Performance Optimization
	•	Location updates batched every 5 seconds
	•	Distance threshold of 10 meters to reduce API calls
	•	Efficient state management with React hooks
	•	Lazy loading of screens
	•	Image optimization for mobile

Security
	•	Secure token storage with Expo Secure Store
	•	HTTPS-only API communication
	•	JWT token validation
	•	Sensitive data encryption
	•	No hardcoded credentials

Troubleshooting
Location Permission Denied
	•	Check iOS/Android settings
	•	Request permissions explicitly
	•	Ensure background location enabled

Notifications Not Working
	•	Verify notification permissions
	•	Check device notification settings
	•	Test with development build

API Connection Issues
	•	Verify API URL in .env
	•	Check network connectivity
	•	Review API logs

Revenue Model
Driver Earnings
	•	Base Fee: $5-$15 per delivery
	•	Distance Bonus: $0.50 per mile
	•	Tips: 100% to driver
	•	Surge Pricing: Up to 2x during peak hours
	•	Referral Bonus: $100 per referred driver

Platform Revenue
	•	Commission: 15-20% from deliveries
	•	Sponsorships: $99-$499/month from dealerships
	•	Advertising: CPM/CPC based
	•	Lead Generation: $25-$100 per lead

Support
For issues or questions:

	•	Email: support@phoenixexpress.com
	•	Phone: 1-800-PHOENIX-1
	•	In-app support chat

License
Proprietary - Phoenix Express © 2024

Version History
v1.0.0 (2024)
	•	Initial release
	•	Core delivery management
	•	Real-time tracking
	•	Earnings system
	•	Profile management
# Trash-Tracker
AI-Powered Waste Classification and Quantification System with Gaming-Style UI

📋 Project Overview
Trash-Tracker-Project is an innovative AI-powered waste management application designed to revolutionize waste sorting and recycling processes. This project leverages cutting-edge machine learning and computer vision technologies to classify and quantify various types of waste in mixed waste scenarios, helping to streamline waste separation in dumpyards and promote environmental sustainability.

✨ Key Features
🎯 AI-Powered Classification
Hybrid CNN + Transformer Model: Advanced deep learning architecture combining EfficientNetB0 backbone with Transformer blocks
Multi-Class Classification: Identifies 6 waste types: cardboard, glass, metal, paper, plastic, and trash
Real-Time Processing: Instant classification results with confidence scores
📊 Quantification & Analytics
Percentage Breakdown: Calculates the percentage composition of each waste type
Visual Progress Bars: Gaming-style animated progress bars for waste type visualization
Historical Tracking: Save and track classification results over time
🎮 Gaming-Style User Interface
Modern Gaming Aesthetics: Neon effects, glowing elements, and animated gradients
Responsive Design: Works seamlessly on desktop and mobile devices
Interactive Elements: Hover effects, animated buttons, and progress indicators
Digital Typography: Orbitron font for a futuristic gaming feel
🌐 Web Application
Django Backend: Robust Python web framework for scalability
Bootstrap Frontend: Modern, responsive UI components
File Upload System: Drag-and-drop image upload with progress tracking
Results Visualization: Beautiful, game-inspired results display
🛠️ Technologies Used
Backend & AI
Django 3.2+: Web framework for backend development
TensorFlow 2.8+: Deep learning framework for model training and inference
Keras: High-level neural network API
EfficientNetB0: Pre-trained CNN backbone for feature extraction
Transformer Architecture: Attention mechanisms for enhanced classification
Frontend & UI
Bootstrap 4.5.2: Responsive CSS framework
Bootstrap Icons: Modern icon library
HTML5/CSS3: Latest web standards
JavaScript: Interactive functionality and animations
Orbitron Font: Gaming-style typography
Data Processing
Pillow: Image processing and manipulation
NumPy: Numerical computing
ImageDataGenerator: Data augmentation for model training
🚀 Installation & Setup
Prerequisites
Python 3.8+
pip (Python package installer)
Git
Step 1: Clone the Repository
git clone https://github.com/meghanakongara0429/Trash-Tracker-Project.git
cd Trash-Tracker-Project
Step 2: Set Up Virtual Environment
# Create virtual environment
python -m venv venv

# Activate virtual environment
# On Windows:
venv\Scripts\activate
# On macOS/Linux:
source venv/bin/activate
Step 3: Install Dependencies
pip install -r requirements.txt
Step 4: Database Setup
cd trashtracker
python manage.py migrate
Step 5: Run the Development Server
python manage.py runserver
Step 6: Access the Application
Open your browser and navigate to: http://127.0.0.1:8000/

🎯 Usage Guide
1. Home Page
Welcome to the gaming-style interface
View project features and overview
Click "Start Classifying" to begin
2. Upload Image
Navigate to the Upload page
Select a waste image (JPG, PNG formats supported)
Watch the animated progress bar during upload
Get instant classification results
3. View Results
See waste type percentages in animated progress bars
View the uploaded image alongside results
Upload another image or return to home
🤖 Model Training
Training Your Own Model
Prepare Dataset: Organize images in folders by waste type
Run Training Script: Use the provided train_and_save_model.py
Save Model: Model will be saved as waste_cnn_model.h5
Deploy: Place the model file in trashtracker/waste/ directory
Model Architecture
Backbone: EfficientNetB0 (pre-trained on ImageNet)
Transformer: Multi-head attention mechanism
Output: 6-class classification + percentage prediction
Input Size: 224x224x3 RGB images
📁 Project Structure
Trash-Tracker-Project/
├── trashtracker/                 # Django project
│   ├── waste/                   # Main app
│   │   ├── templates/          # HTML templates
│   │   ├── views.py           # Django views
│   │   ├── models.py          # Database models
│   │   └── urls.py            # URL routing
│   ├── static/                # Static files
│   ├── media/                 # Uploaded files
│   └── manage.py              # Django management
├── hybrid model.py            # Model architecture
├── mymo.py                    # Training script
├── requirements.txt           # Python dependencies
└── README.md                  # Project documentation
🎨 UI Features
Gaming-Style Elements
Animated Background: Gradient animation with color transitions
Neon Effects: Glowing borders and text shadows
Interactive Cards: Hover effects and scaling animations
Progress Bars: Animated waste type visualization
Digital Typography: Futuristic font styling
Responsive Design
Mobile-Friendly: Optimized for all screen sizes
Touch Support: Gesture-friendly interface
Fast Loading: Optimized assets and caching
🔧 Configuration
Environment Variables
Create a .env file in the project root:

DEBUG=True
SECRET_KEY=your-secret-key-here
DATABASE_URL=sqlite:///db.sqlite3
Model Configuration
Input Size: 224x224 pixels
Classes: 6 waste types
Batch Size: 32 (configurable)
Learning Rate: 1e-4
🤝 Contributing
Fork the repository
Create a feature branch (git checkout -b feature/AmazingFeature)
Commit your changes (git commit -m 'Add some AmazingFeature')
Push to the branch (git push origin feature/AmazingFeature)
Open a Pull Request
📝 License
This project is licensed under the MIT License - see the LICENSE file for details.

🙏 Acknowledgments
TrashNet Dataset: For providing the waste classification dataset
Django Community: For the excellent web framework
TensorFlow Team: For the powerful deep learning framework
Bootstrap Team: For the responsive UI framework

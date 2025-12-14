# Numerical Analysis Portfolio

A comprehensive collection of Jupyter notebooks demonstrating fundamental numerical analysis methods and algorithms. This portfolio covers key topics in calculus, ordinary differential equations (ODEs), and their computational implementations.

## 📊 Project Structure

```
numerical-analysis-portfolio/
├── Calculus/                          # Numerical calculus methods
│   ├── numerical_integration.ipynb     # Integration techniques (Rectangle, Trapezoidal, Simpson's rules)
│   └── root_finding.ipynb              # Root-finding algorithms (Bisection, Newton-Raphson, Secant)
├── ODE/                                # Ordinary differential equation solvers
│   ├── euler_method.ipynb              # Euler's method for first-order ODEs
│   ├── runge_kutta_method.ipynb        # Runge-Kutta methods (orders 1-4)
│   ├── taylor_series_method.ipynb      # Taylor series expansion method
│   ├── adams_bashforth_method.ipynb    # Multistep predictor method with ML optimization
│   ├── milne_method.ipynb              # Predictor-corrector method
│   ├── picard_iterations.ipynb         # Picard's successive approximation method
│   ├── system_of_odes.ipynb            # Solving systems of coupled ODEs
│   └── bvp_ode_by_fdm.ipynb            # Boundary value problems via finite difference method
├── Linear-Algebra/                     # (Empty - ready for linear algebra methods)
├── PDE/                                # (Empty - ready for PDE methods)
├── ENV/                                # Environment configuration
│   └── pde_ml_env.yml                  # Conda environment specification
└── README.md                           # This file
```

## 🔍 Content Overview

### **Calculus Methods** (`Calculus/`)

#### **numerical_integration.ipynb**
- **Rectangle Rules**: Left, right, and midpoint approximations
- **Trapezoidal Rule**: Linear interpolation between points
- **Simpson's Rules**: Parabolic approximation (1/3 and 3/8 variants)
- **Composite Methods**: Convergence analysis and error estimation
- **Visualization**: Graphical comparison of methods with error metrics

#### **root_finding.ipynb**
- **Bisection Method**: Guaranteed convergence, reliability focused
- **Newton-Raphson Method**: Quadratic convergence for smooth functions
- **Secant Method**: Derivative-free approximation
- **Fixed-Point Iteration**: General iterative approach
- **Convergence Analysis**: Rate of convergence and error bounds
- **Visualization**: Function behavior and iteration paths

### **ODE Solvers** (`ODE/`)

#### **euler_method.ipynb**
- **Explicit Euler**: Basic first-order method
- **Implementation**: Step-by-step numerical integration
- **Comparison**: Against analytical solutions
- **Error Analysis**: Local and global truncation errors
- **Variants**: Implicit Euler, semi-implicit schemes

#### **runge_kutta_method.ipynb**
- **RK1 (Euler)**: First-order method
- **RK2 (Midpoint/Heun)**: Second-order methods
- **RK3**: Third-order Runge-Kutta
- **RK4**: Fourth-order (most widely used)
- **Adaptive methods**: Step size control
- **Performance Comparison**: Accuracy vs computational cost
- **Multiple Examples**: Various ODE types

#### **taylor_series_method.ipynb**
- **Taylor Series Expansion**: Power series solutions
- **Automatic Differentiation**: Computing derivatives symbolically
- **Higher-Order Terms**: Improved accuracy through more terms
- **Example Problems**: Various ODE scenarios
- **Convergence Study**: Radius of convergence analysis

#### **adams_bashforth_method.ipynb**
- **Multistep Method**: Using previous steps
- **Adams-Bashforth Predictor**: Explicit formula
- **Adams-Moulton Corrector**: Implicit correction
- **ML Integration**: Physics-informed neural networks (PINNs)
- **PyTorch Implementation**: Deep learning approach to ODEs
- **Hybrid Methods**: Combining classical and neural approaches

#### **milne_method.ipynb**
- **Predictor-Corrector Scheme**: Two-step process
- **Milne's Formula**: 4th-order method
- **Error Estimation**: Local and global error bounds
- **Stability Analysis**: Region of absolute stability
- **Comparison Studies**: Against single-step methods
- **Multiple Examples**: Different initial conditions

#### **picard_iterations.ipynb**
- **Successive Approximations**: Iterative construction of solution
- **Convergence Theory**: Lipschitz conditions and fixed points
- **Symbolic Computation**: Using SymPy for exact solutions
- **Numerical Iteration**: Computing approximations
- **Visualization**: Convergence demonstration
- **Comparison**: With other methods

#### **system_of_odes.ipynb**
- **Vector Formulation**: First-order system representation
- **Runge-Kutta for Systems**: Extending to multi-dimensional problems
- **Predator-Prey Models**: Lotka-Volterra equations
- **Chemical Reactions**: Coupled reaction kinetics
- **Phase Portraits**: Solution trajectories in phase space
- **Stability Analysis**: Eigenvalue-based equilibrium analysis
- **Multiple Systems**: Various biological and physical models

#### **bvp_ode_by_fdm.ipynb**
- **Boundary Value Problems**: Two-point BVP formulation
- **Finite Difference Method**: Discretization approach
- **Linear BVPs**: Tridiagonal matrix solutions
- **Nonlinear BVPs**: Newton's method on discretized problem
- **Shooting Method**: Alternative BVP approach
- **Applications**: Heat transfer, beam deflection, eigenvalue problems
- **Error Analysis**: Convergence with mesh refinement

## 🛠️ Technologies & Libraries

- **Python 3.x**: Core programming language
- **NumPy**: Numerical computations and array operations
- **SciPy**: Advanced numerical algorithms (`scipy.integrate`)
- **SymPy**: Symbolic mathematics and exact solutions
- **Matplotlib**: Data visualization and plotting
- **PyTorch**: Machine learning and neural networks (for PINN examples)
- **Jupyter**: Interactive notebook environment

## 📋 Requirements

### Core Dependencies
```
numpy>=1.21.0
scipy>=1.7.0
sympy>=1.12
matplotlib>=3.4.0
jupyter>=1.0.0
```

### Optional (for ML methods)
```
torch>=1.10.0
```

## 🚀 Getting Started

### 1. Clone or Download
```bash
git clone <repository-url>
cd numerical-analysis-portfolio
```

### 2. Set Up Environment

**Option A: Using Conda**
```bash
conda env create -f ENV/pde_ml_env.yml
conda activate pde_ml_env
```

**Option B: Using pip**
```bash
pip install -r requirements.txt
```

### 3. Launch Jupyter
```bash
jupyter notebook
```

### 4. Open and Explore
Navigate to the notebook of interest and run cells sequentially.

## 📖 How to Use Each Notebook

1. **Read the markdown cells** for context and theory
2. **Execute code cells** in order for proper variable initialization
3. **Modify parameters** to experiment with different problem configurations
4. **Study visualizations** to understand algorithm behavior
5. **Compare methods** side-by-side using provided comparison cells

## 🎯 Key Topics by Difficulty

### Beginner
- Root Finding: Bisection Method
- Numerical Integration: Rectangle Rules
- Euler Method for ODEs

### Intermediate
- Newton-Raphson Method
- Simpson's Rules
- Runge-Kutta Methods (RK2, RK3)
- Systems of ODEs

### Advanced
- Runge-Kutta Order 4 with Adaptive Stepping
- Adams-Bashforth Multistep Methods
- Physics-Informed Neural Networks (PINNs)
- Nonlinear Boundary Value Problems
- Predictor-Corrector Schemes

## 📊 Notebook Statistics

| Category | Files | Total Methods |
|----------|-------|----------------|
| Calculus | 2 | 8+ |
| ODE Solvers | 8 | 15+ |
| Total | 10 | 23+ |

## ✨ Features

- ✅ Detailed theoretical background in markdown cells
- ✅ Complete working implementations
- ✅ Comparison with analytical solutions where available
- ✅ Error analysis and convergence studies
- ✅ High-quality visualizations
- ✅ Practical examples from physics and engineering
- ✅ Machine learning integration (PINN examples)
- ✅ Ready-to-run code with minimal dependencies

## 🔬 Example Applications

The notebooks solve real-world problems including:

- **Physics**: Projectile motion, spring-mass systems, heat diffusion
- **Biology**: Predator-prey dynamics (Lotka-Volterra)
- **Chemistry**: Reaction kinetics and rate equations
- **Engineering**: Beam deflection, heat transfer
- **Population Dynamics**: Growth models

## 📚 Learning Path

**Recommended progression:**
1. Start with `Calculus/root_finding.ipynb` (fundamental concepts)
2. Move to `Calculus/numerical_integration.ipynb` (similar difficulty)
3. Progress to `ODE/euler_method.ipynb` (introduce ODEs)
4. Explore `ODE/runge_kutta_method.ipynb` (improved methods)
5. Study `ODE/system_of_odes.ipynb` (real applications)
6. Advanced: `ODE/adams_bashforth_method.ipynb` (multistep methods)
7. Advanced: `ODE/bvp_ode_by_fdm.ipynb` (BVPs and FDM)

## 🐛 Troubleshooting

### ImportError for libraries
```bash
pip install numpy scipy sympy matplotlib jupyter
```

### Permission issues with notebooks
```bash
jupyter notebook --no-browser
```

### SymPy slow on first import
This is normal; subsequent imports are faster.

## 📝 Notes

- Empty folders (`Linear-Algebra/`, `PDE/`) are reserved for future expansion
- Corrupted backup files in `ODE/` can be ignored
- All notebooks are self-contained and can be run independently
- Each notebook saves its outputs for later reference

## 🤝 Contributing

Suggestions and improvements are welcome! Consider:
- Adding more numerical methods
- Expanding applications
- Improving visualizations
- Adding performance benchmarks

## 📄 License

This portfolio is provided as-is for educational purposes.

## 🎓 Educational Use

This portfolio is ideal for:
- Students learning numerical analysis
- Researchers exploring different ODE solvers
- Educators creating course materials
- Practitioners comparing numerical methods

---

**Last Updated**: December 2024  
**Python Version**: 3.8+  
**Status**: Active and maintained
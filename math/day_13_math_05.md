# Day 13: Math(Wrap-up)
## Coordinate
## Transform matrix : make a scaling and rotate
## Code : 
 • sp.ndimage.affine_transform
 • E = np.vstack([e1, e2]).T
## 고유분해 Eigen - decomposition :  square matrix  
 • E = np.array([[2,3], [2,1]])
 • eig_val = np.linalg.eig(E)
 • eig_val # colum is vector!
## AV = VΛ (A have inverse) VΛV-1
## 특이분해
## Symmetric matrix by real-number have real-number Eigen-value and Eigen Vector is ortho-normal each others
## Scatter Matrix : eigen value is Positive semi-definate

			from sklearn.datasets import load_boston 
			boston = load_boston()
			X = boston.data
			COV = X.T @ X  #  <--------------------순서주의 !!!!!
			w, V = np.linalg.eig(COV) 
			w

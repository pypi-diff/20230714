# Comparing `tmp/neuropop-0.1.tar.gz` & `tmp/neuropop-1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neuropop-0.1.tar", last modified: Mon Mar 27 18:26:23 2023, max compression
+gzip compressed data, was "neuropop-1.0.tar", last modified: Fri Jul 14 13:07:44 2023, max compression
```

## Comparing `neuropop-0.1.tar` & `neuropop-1.0.tar`

### file list

```diff
@@ -1,20 +1,36 @@
-drwxrwxrwx   0        0        0        0 2023-03-27 18:26:23.809654 neuropop-0.1/
--rw-rw-rw-   0        0        0      524 2023-03-27 18:26:23.808654 neuropop-0.1/PKG-INFO
--rw-rw-rw-   0        0        0       62 2023-03-27 15:52:04.000000 neuropop-0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-03-27 18:26:23.798655 neuropop-0.1/neuropop/
--rw-rw-rw-   0        0        0     5190 2023-03-27 17:28:31.000000 neuropop-0.1/neuropop/dimensionality.py
--rw-rw-rw-   0        0        0     5423 2023-03-27 16:00:26.000000 neuropop-0.1/neuropop/filtering.py
--rw-rw-rw-   0        0        0     4301 2023-03-27 16:28:40.000000 neuropop-0.1/neuropop/future_prediction.py
--rw-rw-rw-   0        0        0     8417 2023-03-27 16:43:38.000000 neuropop-0.1/neuropop/linear_prediction.py
--rw-rw-rw-   0        0        0    18247 2023-03-27 16:44:46.000000 neuropop-0.1/neuropop/nn_prediction.py
--rw-rw-rw-   0        0        0     1237 2023-03-27 17:26:32.000000 neuropop-0.1/neuropop/peer_prediction.py
--rw-rw-rw-   0        0        0     6084 2023-03-27 16:33:27.000000 neuropop-0.1/neuropop/split_data.py
--rw-rw-rw-   0        0        0     3433 2023-03-27 16:33:01.000000 neuropop-0.1/neuropop/utils.py
-drwxrwxrwx   0        0        0        0 2023-03-27 18:26:23.807654 neuropop-0.1/neuropop.egg-info/
--rw-rw-rw-   0        0        0      524 2023-03-27 18:26:23.000000 neuropop-0.1/neuropop.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      381 2023-03-27 18:26:23.000000 neuropop-0.1/neuropop.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-27 18:26:23.000000 neuropop-0.1/neuropop.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       97 2023-03-27 18:26:23.000000 neuropop-0.1/neuropop.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2023-03-27 18:26:23.000000 neuropop-0.1/neuropop.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-03-27 18:26:23.809654 neuropop-0.1/setup.cfg
--rw-rw-rw-   0        0        0     1432 2023-03-27 18:25:59.000000 neuropop-0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 13:07:44.878613 neuropop-1.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 13:07:44.874613 neuropop-1.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 13:07:44.874613 neuropop-1.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1854 2023-07-14 13:07:28.000000 neuropop-1.0/.github/workflows/test_and_deploy.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-14 13:07:28.000000 neuropop-1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     6169 2023-07-14 13:07:44.878613 neuropop-1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5691 2023-07-14 13:07:28.000000 neuropop-1.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2150 2023-07-14 13:07:28.000000 neuropop-1.0/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 13:07:44.878613 neuropop-1.0/figures/
+-rw-r--r--   0 runner    (1001) docker     (123)    87394 2023-07-14 13:07:28.000000 neuropop-1.0/figures/SVCA.PNG
+-rw-r--r--   0 runner    (1001) docker     (123)    70690 2023-07-14 13:07:28.000000 neuropop-1.0/figures/cvPCA.PNG
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-14 13:07:28.000000 neuropop-1.0/figures/figsfromrefs
+-rw-r--r--   0 runner    (1001) docker     (123)   380397 2023-07-14 13:07:28.000000 neuropop-1.0/figures/nn_prediction.PNG
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 13:07:44.878613 neuropop-1.0/neuropop/
+-rw-r--r--   0 runner    (1001) docker     (123)     5123 2023-07-14 13:07:28.000000 neuropop-1.0/neuropop/dimensionality.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4019 2023-07-14 13:07:28.000000 neuropop-1.0/neuropop/filtering.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4301 2023-07-14 13:07:28.000000 neuropop-1.0/neuropop/future_prediction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8827 2023-07-14 13:07:28.000000 neuropop-1.0/neuropop/linear_prediction.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19862 2023-07-14 13:07:28.000000 neuropop-1.0/neuropop/nn_prediction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1320 2023-07-14 13:07:28.000000 neuropop-1.0/neuropop/peer_prediction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6083 2023-07-14 13:07:28.000000 neuropop-1.0/neuropop/split_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3433 2023-07-14 13:07:28.000000 neuropop-1.0/neuropop/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 13:07:44.878613 neuropop-1.0/neuropop.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6169 2023-07-14 13:07:44.000000 neuropop-1.0/neuropop.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      612 2023-07-14 13:07:44.000000 neuropop-1.0/neuropop.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 13:07:44.000000 neuropop-1.0/neuropop.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-14 13:07:44.000000 neuropop-1.0/neuropop.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 13:07:44.000000 neuropop-1.0/neuropop.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-14 13:07:44.878613 neuropop-1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1229 2023-07-14 13:07:28.000000 neuropop-1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 13:07:44.878613 neuropop-1.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     3573 2023-07-14 13:07:28.000000 neuropop-1.0/tests/make_test.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)      312 2023-07-14 13:07:28.000000 neuropop-1.0/tests/test_dim.py
+-rw-r--r--   0 runner    (1001) docker     (123)      976 2023-07-14 13:07:28.000000 neuropop-1.0/tests/test_linpred.py
+-rw-r--r--   0 runner    (1001) docker     (123)      819 2023-07-14 13:07:28.000000 neuropop-1.0/tests/test_nnpred.py
+-rw-r--r--   0 runner    (1001) docker     (123)      695 2023-07-14 13:07:28.000000 neuropop-1.0/tox.ini
```

### Comparing `neuropop-0.1/neuropop/dimensionality.py` & `neuropop-1.0/neuropop/dimensionality.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,176 +1,179 @@
-import numpy as np
-from scipy.interpolate import interp1d
-from scipy.ndimage import gaussian_filter1d
-from scipy.optimize import curve_fit
-
-def fit_asymptote(x, y, xall, fitexp=False):
-    from sklearn.linear_model import LinearRegression
-    ''' fit y = alpha + beta / sqrt(x)'''
-    xi = x.copy()**-0.5
-    if xi.ndim < 2:
-        xi = xi[:,np.newaxis]
-        xall = xall[:,np.newaxis]
-    reg = LinearRegression().fit(xi, y)
-    beta = reg.coef_
-    alpha = reg.intercept_
-    r2 = reg.score(xi, y)
-    if not fitexp:
-        ypred = alpha + np.dot(xall**-0.5, beta)
-        par = [alpha]
-        for b in beta:
-            par.append(b)
-        return par, r2, ypred
-    if xi.shape[1]==1:
-        par0 = [alpha, beta[0], 0.5]
-        f = asymp
-    else:
-        par0 = [alpha, beta[0], beta[1], 0.5, 0.5]
-        f = asymp2
-    par, mcov = curve_fit(f, x, y, par0)
-
-    if xi.shape[1]==1:
-        ypred = asymp(x, par[0], par[1], par[2])
-    else:
-        ypred = asymp2(x.T, par[0], par[1], par[2], par[3], par[4])
-    r2 = np.corrcoef(ypred, y)[0,1]
-    print(par, r2)
-    if xi.shape[1]==1:
-        ypred = asymp(xall, par[0], par[1], par[2])
-    else:
-        ypred = asymp2(xall.T, par[0], par[1], par[2], par[3], par[4])
-    return par, r2**2, ypred
-
-def asymp(x, alpha, beta, t1):
-    y = alpha + beta / x**t1
-    return y
-
-def asymp2(x, alpha, beta, gamma, t1, t2):
-    y = alpha + beta / x[0]**t1 + gamma / x[1]**t2
-    return y
-
-def discrimination_threshold(P, x):
-    P = (P + 1-P[::-1])/2
-    par0 = np.array([5])
-    par, mcov = curve_fit(logistic, x, P, par0)
-    p75 = - np.log(1/0.75 - 1) * par[0]
-    return p75, logistic(x, par)
-
-# psychometric function
-def logistic(x, beta):
-    return 1. / (1 + np.exp( -x / beta ))
-
-def get_powerlaw(ss, trange):
-    logss = np.log(np.abs(ss))
-    y = logss[trange][:,np.newaxis]
-    trange += 1
-    nt = trange.size
-    x = np.concatenate((-np.log(trange)[:,np.newaxis], np.ones((nt,1))), axis=1)
-    w = 1.0 / trange.astype(np.float32)[:,np.newaxis]
-    b = np.linalg.solve(x.T @ (x * w), (w * x).T @ y).flatten()
-
-    allrange = np.arange(0, ss.size).astype(int) + 1
-    x = np.concatenate((-np.log(allrange)[:,np.newaxis], np.ones((ss.size,1))), axis=1)
-    ypred = np.exp((x * b).sum(axis=1))
-    alpha = b[0]
-    return alpha,ypred
-
-def shuff_cvPCA(X, nshuff=10):
-    ''' X is 2 x stimuli x neurons '''
-    nc = min(1024, X.shape[1])
-
-    nr = X.shape[0]
-
-    ss=np.zeros((nshuff,nc))
-    for k in range(nshuff):
-        rperm = np.random.rand(X.shape[1])
-        iflip = rperm > 0.5
-        #X0 = np.float64(X.copy())
-        X0 = np.roll(X, k, axis=0)
-
-        for t in range(nr):
-            X0[t,iflip] = X[(t+1)%nr,iflip]
-            #X0[1,iflip] = X[0,iflip]
-
-        ss[k]=cvPCA(X0)
-    return ss
-
-def repscvPCA(A,B, nshuff=10):
-    NC, NN = A.shape
-    ss = np.zeros((nshuff, NC))
-    for n in range(nshuff):
-        ss[n] = scvPCA(A,B)
-    return ss
-
-def scvPCA(A, B):
-    """ A, B are neurons x stimuli, NC is # of eigenvalues to return """
-    NC, NN = A.shape
-
-    rperm = np.random.permutation(NN)
-
-    A1 = A[:,rperm[:NN//2]]
-    B1 = B[:,rperm[:NN//2]]
-
-    A2 = A[:,rperm[NN//2:]]
-    B2 = B[:,rperm[NN//2:]]
-
-    covAB = A1 @ B1.T
-    u,s,v = np.linalg.svd(covAB, full_matrices=False)
-    covAB2 = A2 @ B2.T
-    e_AB = np.sum(u  * (covAB2 @ u), axis=0)
-    return e_AB
-
-def cvPCA(X):
-    ''' X is 2 x stimuli x neurons '''
-    nr = X.shape[0]
-    pca = PCA(n_components=min(1024, X.shape[1])).fit(X[0])
-    #u = pca.components_.T
-    #sv = pca.singular_values_
-    #xproj = X[0].T @ (u / sv)
-
-    xproj = pca.components_.T
-    cproj0 = X[-2] @ xproj
-    cproj1 = X[-1] @ xproj
-    ss = (cproj0 * cproj1).sum(axis=0)
-    return ss
-
-def SVCA(X):
-    from sklearn.decomposition import PCA
-    # compute power law
-    # SVCA
-    #X -= X.mean(axis=1)[:,np.newaxis]
-
-    NN,NT = X.shape
-
-    # split cells into test and train
-    norder = np.random.permutation(NN)
-    nhalf = int(norder.size/2)
-    ntrain = norder[:nhalf]
-    ntest = norder[nhalf:]
-
-    # split time into test and train
-    torder = np.random.permutation(NT)
-    thalf = int(torder.size/2)
-    ttrain = torder[:thalf]
-    ttest = torder[thalf:]
-    #if ntrain.size > ttrain.size:
-    #    cov = X[np.ix_(ntrain, ttrain)].T @ X[np.ix_(ntest, ttrain)]
-    #    u,sv,v = svdecon(cov, k=min(1024, nhalf-1))
-    #    u = X[np.ix_(ntrain, ttrain)] @ u
-    #    u /= (u**2).sum(axis=0)**0.5
-    #    v = X[np.ix_(ntest, ttrain)] @ v
-    #    v /= (v**2).sum(axis=0)**0.5
-    #else:
-    cov = X[np.ix_(ntrain, ttrain)] @ X[np.ix_(ntest, ttrain)].T
-    u = PCA(n_components=min(1024, nhalf-1), svd_solver='randomized').fit_transform(cov)
-    u /= (u**2).sum(axis=0)**0.5
-    v = cov.T @ u
-    v /= (v**2).sum(axis=0)**0.5
-
-    strain = u.T @ X[np.ix_(ntrain,ttest)]
-    stest = v.T @ X[np.ix_(ntest,ttest)]
-
-    # covariance k is uk.T * F * G.T * vk / npts
-    scov = (strain * stest).mean(axis=1)
-    varcov = (strain**2 + stest**2).mean(axis=1) / 2
-
-    return scov, varcov
+"""
+Copright © 2023 Howard Hughes Medical Institute, Authored by Carsen Stringer and Marius Pachitariu.
+"""
+import numpy as np
+from scipy.interpolate import interp1d
+from scipy.ndimage import gaussian_filter1d
+from scipy.optimize import curve_fit
+
+def fit_asymptote(x, y, xall, fitexp=False):
+    from sklearn.linear_model import LinearRegression
+    ''' fit y = alpha + beta / sqrt(x)'''
+    xi = x.copy()**-0.5
+    if xi.ndim < 2:
+        xi = xi[:,np.newaxis]
+        xall = xall[:,np.newaxis]
+    reg = LinearRegression().fit(xi, y)
+    beta = reg.coef_
+    alpha = reg.intercept_
+    r2 = reg.score(xi, y)
+    if not fitexp:
+        ypred = alpha + np.dot(xall**-0.5, beta)
+        par = [alpha]
+        for b in beta:
+            par.append(b)
+        return par, r2, ypred
+    if xi.shape[1]==1:
+        par0 = [alpha, beta[0], 0.5]
+        f = asymp
+    else:
+        par0 = [alpha, beta[0], beta[1], 0.5, 0.5]
+        f = asymp2
+    par, mcov = curve_fit(f, x, y, par0)
+
+    if xi.shape[1]==1:
+        ypred = asymp(x, par[0], par[1], par[2])
+    else:
+        ypred = asymp2(x.T, par[0], par[1], par[2], par[3], par[4])
+    r2 = np.corrcoef(ypred, y)[0,1]
+    print(par, r2)
+    if xi.shape[1]==1:
+        ypred = asymp(xall, par[0], par[1], par[2])
+    else:
+        ypred = asymp2(xall.T, par[0], par[1], par[2], par[3], par[4])
+    return par, r2**2, ypred
+
+def asymp(x, alpha, beta, t1):
+    y = alpha + beta / x**t1
+    return y
+
+def asymp2(x, alpha, beta, gamma, t1, t2):
+    y = alpha + beta / x[0]**t1 + gamma / x[1]**t2
+    return y
+
+def discrimination_threshold(P, x):
+    P = (P + 1-P[::-1])/2
+    par0 = np.array([5])
+    par, mcov = curve_fit(logistic, x, P, par0)
+    p75 = - np.log(1/0.75 - 1) * par[0]
+    return p75, logistic(x, par)
+
+# psychometric function
+def logistic(x, beta):
+    return 1. / (1 + np.exp( -x / beta ))
+
+def get_powerlaw(ss, trange):
+    logss = np.log(np.abs(ss))
+    y = logss[trange][:,np.newaxis]
+    trange += 1
+    nt = trange.size
+    x = np.concatenate((-np.log(trange)[:,np.newaxis], np.ones((nt,1))), axis=1)
+    w = 1.0 / trange.astype(np.float32)[:,np.newaxis]
+    b = np.linalg.solve(x.T @ (x * w), (w * x).T @ y).flatten()
+
+    allrange = np.arange(0, ss.size).astype(int) + 1
+    x = np.concatenate((-np.log(allrange)[:,np.newaxis], np.ones((ss.size,1))), axis=1)
+    ypred = np.exp((x * b).sum(axis=1))
+    alpha = b[0]
+    return alpha,ypred
+
+def shuff_cvPCA(X, nshuff=10):
+    ''' X is 2 x stimuli x neurons '''
+    nc = min(1024, X.shape[1])
+
+    nr = X.shape[0]
+
+    ss=np.zeros((nshuff,nc))
+    for k in range(nshuff):
+        rperm = np.random.rand(X.shape[1])
+        iflip = rperm > 0.5
+        #X0 = np.float64(X.copy())
+        X0 = np.roll(X, k, axis=0)
+
+        for t in range(nr):
+            X0[t,iflip] = X[(t+1)%nr,iflip]
+            #X0[1,iflip] = X[0,iflip]
+
+        ss[k]=cvPCA(X0)
+    return ss
+
+def repscvPCA(A,B, nshuff=10):
+    NC, NN = A.shape
+    ss = np.zeros((nshuff, NC))
+    for n in range(nshuff):
+        ss[n] = scvPCA(A,B)
+    return ss
+
+def scvPCA(A, B):
+    """ A, B are neurons x stimuli, NC is # of eigenvalues to return """
+    NC, NN = A.shape
+
+    rperm = np.random.permutation(NN)
+
+    A1 = A[:,rperm[:NN//2]]
+    B1 = B[:,rperm[:NN//2]]
+
+    A2 = A[:,rperm[NN//2:]]
+    B2 = B[:,rperm[NN//2:]]
+
+    covAB = A1 @ B1.T
+    u,s,v = np.linalg.svd(covAB, full_matrices=False)
+    covAB2 = A2 @ B2.T
+    e_AB = np.sum(u  * (covAB2 @ u), axis=0)
+    return e_AB
+
+def cvPCA(X):
+    ''' X is 2 x stimuli x neurons '''
+    nr = X.shape[0]
+    pca = PCA(n_components=min(1024, X.shape[1])).fit(X[0])
+    #u = pca.components_.T
+    #sv = pca.singular_values_
+    #xproj = X[0].T @ (u / sv)
+
+    xproj = pca.components_.T
+    cproj0 = X[-2] @ xproj
+    cproj1 = X[-1] @ xproj
+    ss = (cproj0 * cproj1).sum(axis=0)
+    return ss
+
+def SVCA(X):
+    from sklearn.decomposition import PCA
+    # compute power law
+    # SVCA
+    #X -= X.mean(axis=1)[:,np.newaxis]
+
+    NN,NT = X.shape
+
+    # split cells into test and train
+    norder = np.random.permutation(NN)
+    nhalf = int(norder.size/2)
+    ntrain = norder[:nhalf]
+    ntest = norder[nhalf:]
+
+    # split time into test and train
+    torder = np.random.permutation(NT)
+    thalf = int(torder.size/2)
+    ttrain = torder[:thalf]
+    ttest = torder[thalf:]
+    #if ntrain.size > ttrain.size:
+    #    cov = X[np.ix_(ntrain, ttrain)].T @ X[np.ix_(ntest, ttrain)]
+    #    u,sv,v = svdecon(cov, k=min(1024, nhalf-1))
+    #    u = X[np.ix_(ntrain, ttrain)] @ u
+    #    u /= (u**2).sum(axis=0)**0.5
+    #    v = X[np.ix_(ntest, ttrain)] @ v
+    #    v /= (v**2).sum(axis=0)**0.5
+    #else:
+    cov = X[np.ix_(ntrain, ttrain)] @ X[np.ix_(ntest, ttrain)].T
+    u = PCA(n_components=min(1024, nhalf-1), svd_solver='randomized').fit_transform(cov)
+    u /= (u**2).sum(axis=0)**0.5
+    v = cov.T @ u
+    v /= (v**2).sum(axis=0)**0.5
+
+    strain = u.T @ X[np.ix_(ntrain,ttest)]
+    stest = v.T @ X[np.ix_(ntest,ttest)]
+
+    # covariance k is uk.T * F * G.T * vk / npts
+    scov = (strain * stest).mean(axis=1)
+    varcov = (strain**2 + stest**2).mean(axis=1) / 2
+
+    return scov, varcov
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `neuropop-0.1/neuropop/future_prediction.py` & `neuropop-1.0/neuropop/future_prediction.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,110 +1,113 @@
-import numpy as np 
-import torch
-from torch.nn.functional import conv1d
-from utils import compute_varexp
-
-def causal_filter(X, swave, tlag, remove_start=False, device=torch.device('cuda')):
-    """ filter matrix X (n_channels, (n_batches,) n_time) with filters swave
-    
-    returns Xfilt (n_out, n_batches*n_time)
-    """
-    if X.ndim < 3:
-        X = X.unsqueeze(1)
-    NT = X.shape[-1]
-    nt =  swave.shape[1]
-    # reshape X for input to be (n_channels*n_batches, 1, n_time)
-    Xfilt = conv1d(X.reshape(-1, X.shape[-1]).unsqueeze(1), 
-                   swave.unsqueeze(1), padding=nt+tlag)
-    Xfilt = Xfilt[..., :NT]
-    Xfilt = Xfilt[..., nt:] if remove_start else Xfilt
-    Xfilt = Xfilt.reshape(X.shape[0], X.shape[1], swave.shape[0], -1)
-    Xfilt = Xfilt.permute(0,2,1,3)
-    Xfilt = Xfilt.reshape(X.shape[0]*swave.shape[0], X.shape[1], -1)
-    return Xfilt
-
-def fit_causal_prediction(X_train, X_test, swave, lam = 1e-3, tlag=1, device=torch.device('cuda')):
-    """ predict X in the future with exponential filters"""
-    # fit on train data
-    Xfilt = causal_filter(X_train, swave, tlag)    
-    Xfilt = Xfilt.reshape(Xfilt.shape[0], -1)
-    NT = X_train.shape[1] * X_train.shape[2]
-    nff = Xfilt.shape[0]
-    CC = (Xfilt @ Xfilt.T)/NT + lam * torch.eye(nff, device = device)
-    CX = (Xfilt @ X_train.reshape(-1,NT).T) / NT
-    B = torch.linalg.solve(CC, CX)    
-
-    # performance on test data
-    Xfilt = causal_filter(X_test, swave, tlag, remove_start=True)    
-    Xfilt = Xfilt.reshape(Xfilt.shape[0], -1)
-    ypred = B.T @ Xfilt
-    nt = swave.shape[1]
-    ve = compute_varexp(X_test[:,:,nt:].reshape(X_test.shape[0],-1).T, ypred.T)
-    return ve, ypred, B
-
-def future_prediction(X, Ball, swave, device=torch.device('cuda')):
-    """ create future prediction """
-    tlag = Ball.shape[-1]
-    Xfilt = causal_filter(X, swave, tlag, remove_start=True)
-    vef = np.zeros((X.shape[0], tlag))
-    nt = swave.shape[1]
-    Xpred = np.zeros((X.shape[0], X.shape[1], X.shape[2]-nt, tlag))
-    for k in range(tlag):
-        Xfilt0 = Xfilt[:,:,tlag-k:].reshape(Xfilt.shape[0], -1)
-        B = torch.from_numpy(Ball[:,:,k]).to(device)
-        ypred = (B.T @ Xfilt0)
-        ve = compute_varexp(X[:,:,nt:-(tlag-k)].reshape(X.shape[0],-1).T, 
-                                        ypred.T)
-        ypred = ypred.reshape(X.shape[0], X.shape[1], -1)
-        vef[:,k] = ve.cpu().numpy()
-        Xpred[:,:,:-(tlag-k),k] = ypred.cpu().numpy()
-    return vef, Xpred
-
-def predict_future(x, keypoint_labels=None, get_future=True, lam=1e-3, device=torch.device('cuda')):
-    """ predict keypoints or latents in future
-    
-    x is (n_time, n_keypoints) and z-scored per keypoint
-    
-    """
-    nt = 128
-    sigs = torch.FloatTensor(2**np.arange(0,8,1)).unsqueeze(-1)
-    swave = torch.exp( - torch.arange(nt) / sigs).to(device)
-    swave = torch.flip(swave, [1])
-    swave = swave / (swave**2).sum(1, keepdim=True)**.5
-
-    tlags = np.arange(1, 501, 1)
-    tlags = np.append(tlags, np.arange(525, 2000, 25))
-
-    X = torch.from_numpy(x.T).float().to(device)
-
-    itrain, itest = split_traintest(len(x), frac=0.25, pad=nt)
-
-    X_train = X[:,itrain]
-    X_test = X[:,itest]
-
-    n_kp = X_train.shape[0]
-    n_tlags = len(tlags)
-    vet = np.zeros((n_kp, n_tlags), 'float32')
-    Ball = np.zeros((swave.shape[0]*n_kp, n_kp, n_tlags), 'float32')
-    for k,tlag in enumerate(tlags):
-        ve, ypred, B = fit_causal_prediction(X_train, X_test, swave, tlag=tlag, lam=lam)
-        vet[:,k] = ve.cpu().numpy()
-        Ball[:,:,k] = B.cpu().numpy()
-        
-    if get_future:
-        vef, ypred = future_prediction(X_test, Ball[:,:,:500], swave)
-    else:
-        ypred = None
-
-    if keypoint_labels is not None:
-        # tile for X and Y
-        kp_labels = np.tile(np.array(keypoint_labels)[:,np.newaxis], (1,2)).flatten()
-
-        areas = ['eye', 'whisker', 'nose']
-        vet_area = np.zeros((len(areas), vet.shape[1]))
-        for j in range(len(areas)):
-            ak = np.array([k for k in range(len(kp_labels)) if areas[j] in kp_labels[k]])
-            vet_area[j] = vet[ak].mean(axis=0)
-    else:
-        vet_area = None
-
+"""
+Copright © 2023 Howard Hughes Medical Institute, Authored by Carsen Stringer and Marius Pachitariu.
+"""
+import numpy as np 
+import torch
+from torch.nn.functional import conv1d
+from utils import compute_varexp
+
+def causal_filter(X, swave, tlag, remove_start=False, device=torch.device('cuda')):
+    """ filter matrix X (n_channels, (n_batches,) n_time) with filters swave
+    
+    returns Xfilt (n_out, n_batches*n_time)
+    """
+    if X.ndim < 3:
+        X = X.unsqueeze(1)
+    NT = X.shape[-1]
+    nt =  swave.shape[1]
+    # reshape X for input to be (n_channels*n_batches, 1, n_time)
+    Xfilt = conv1d(X.reshape(-1, X.shape[-1]).unsqueeze(1), 
+                   swave.unsqueeze(1), padding=nt+tlag)
+    Xfilt = Xfilt[..., :NT]
+    Xfilt = Xfilt[..., nt:] if remove_start else Xfilt
+    Xfilt = Xfilt.reshape(X.shape[0], X.shape[1], swave.shape[0], -1)
+    Xfilt = Xfilt.permute(0,2,1,3)
+    Xfilt = Xfilt.reshape(X.shape[0]*swave.shape[0], X.shape[1], -1)
+    return Xfilt
+
+def fit_causal_prediction(X_train, X_test, swave, lam = 1e-3, tlag=1, device=torch.device('cuda')):
+    """ predict X in the future with exponential filters"""
+    # fit on train data
+    Xfilt = causal_filter(X_train, swave, tlag)    
+    Xfilt = Xfilt.reshape(Xfilt.shape[0], -1)
+    NT = X_train.shape[1] * X_train.shape[2]
+    nff = Xfilt.shape[0]
+    CC = (Xfilt @ Xfilt.T)/NT + lam * torch.eye(nff, device = device)
+    CX = (Xfilt @ X_train.reshape(-1,NT).T) / NT
+    B = torch.linalg.solve(CC, CX)    
+
+    # performance on test data
+    Xfilt = causal_filter(X_test, swave, tlag, remove_start=True)    
+    Xfilt = Xfilt.reshape(Xfilt.shape[0], -1)
+    ypred = B.T @ Xfilt
+    nt = swave.shape[1]
+    ve = compute_varexp(X_test[:,:,nt:].reshape(X_test.shape[0],-1).T, ypred.T)
+    return ve, ypred, B
+
+def future_prediction(X, Ball, swave, device=torch.device('cuda')):
+    """ create future prediction """
+    tlag = Ball.shape[-1]
+    Xfilt = causal_filter(X, swave, tlag, remove_start=True)
+    vef = np.zeros((X.shape[0], tlag))
+    nt = swave.shape[1]
+    Xpred = np.zeros((X.shape[0], X.shape[1], X.shape[2]-nt, tlag))
+    for k in range(tlag):
+        Xfilt0 = Xfilt[:,:,tlag-k:].reshape(Xfilt.shape[0], -1)
+        B = torch.from_numpy(Ball[:,:,k]).to(device)
+        ypred = (B.T @ Xfilt0)
+        ve = compute_varexp(X[:,:,nt:-(tlag-k)].reshape(X.shape[0],-1).T, 
+                                        ypred.T)
+        ypred = ypred.reshape(X.shape[0], X.shape[1], -1)
+        vef[:,k] = ve.cpu().numpy()
+        Xpred[:,:,:-(tlag-k),k] = ypred.cpu().numpy()
+    return vef, Xpred
+
+def predict_future(x, keypoint_labels=None, get_future=True, lam=1e-3, device=torch.device('cuda')):
+    """ predict keypoints or latents in future
+    
+    x is (n_time, n_keypoints) and z-scored per keypoint
+    
+    """
+    nt = 128
+    sigs = torch.FloatTensor(2**np.arange(0,8,1)).unsqueeze(-1)
+    swave = torch.exp( - torch.arange(nt) / sigs).to(device)
+    swave = torch.flip(swave, [1])
+    swave = swave / (swave**2).sum(1, keepdim=True)**.5
+
+    tlags = np.arange(1, 501, 1)
+    tlags = np.append(tlags, np.arange(525, 2000, 25))
+
+    X = torch.from_numpy(x.T).float().to(device)
+
+    itrain, itest = split_traintest(len(x), frac=0.25, pad=nt)
+
+    X_train = X[:,itrain]
+    X_test = X[:,itest]
+
+    n_kp = X_train.shape[0]
+    n_tlags = len(tlags)
+    vet = np.zeros((n_kp, n_tlags), 'float32')
+    Ball = np.zeros((swave.shape[0]*n_kp, n_kp, n_tlags), 'float32')
+    for k,tlag in enumerate(tlags):
+        ve, ypred, B = fit_causal_prediction(X_train, X_test, swave, tlag=tlag, lam=lam)
+        vet[:,k] = ve.cpu().numpy()
+        Ball[:,:,k] = B.cpu().numpy()
+        
+    if get_future:
+        vef, ypred = future_prediction(X_test, Ball[:,:,:500], swave)
+    else:
+        ypred = None
+
+    if keypoint_labels is not None:
+        # tile for X and Y
+        kp_labels = np.tile(np.array(keypoint_labels)[:,np.newaxis], (1,2)).flatten()
+
+        areas = ['eye', 'whisker', 'nose']
+        vet_area = np.zeros((len(areas), vet.shape[1]))
+        for j in range(len(areas)):
+            ak = np.array([k for k in range(len(kp_labels)) if areas[j] in kp_labels[k]])
+            vet_area[j] = vet[ak].mean(axis=0)
+    else:
+        vet_area = None
+
     return vet, vet_area, tlags, ypred, itest[:, nt:]
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `neuropop-0.1/neuropop/linear_prediction.py` & `neuropop-1.0/neuropop/linear_prediction.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,223 +1,242 @@
-import numpy as np 
-import torch
-
-from utils import compute_varexp, bin1d, resample_data
-from split_data import split_traintest
-
-
-def ridge_regression(X, Y, lam=0):
-    """predict Y from X using regularized linear regression using torch arrays
-    *** subtract mean from X and Y before predicting
-    Prediction:
-    >>> Y_pred = X @ A
-    Parameters
-    ----------
-    X : 2D array, input data (n_samples, n_features)
-    Y : 2D array, data to predict (n_samples, n_predictors)
-    Returns
-    --------
-    A : 2D array - prediction matrix 1 (n_predictors, rank)
-    """
-    CXX = (X.T @ X + lam * np.eye(X.shape[1])) / X.shape[0]
-    CXY = (X.T @ Y) / X.shape[0]
-    A = torch.linalg.solve(CXX, CXY)
-    return A
-
-def reduced_rank_regression(X, Y, rank=None, lam=0):
-    """predict Y from X using regularized reduced rank regression using torch arrays
-    *** subtract mean from X and Y before predicting
-    if rank is None, returns A and B of full-rank (minus one) prediction
-    Prediction:
-    >>> Y_pred = X @ B @ A.T
-    Parameters
-    ----------
-    X : 2D array, input data, float32 torch tensor (n_samples, n_features)
-    Y : 2D array, data to predict, float32 torch tensor (n_samples, n_predictors)
-    rank : int (optional, default None)
-        rank to compute reduced rank regression for
-    lam : float (optional, default 0)
-        regularizer
-    Returns
-    --------
-    A : 2D array - prediction matrix 1 (n_predictors, rank)
-    B : 2D array - prediction matrix 2 (n_features, rank)
-    """
-    min_dim = min(Y.shape[1], min(X.shape[0], X.shape[1])) - 1
-    if rank is None:
-        rank = min_dim
-    else:
-        rank = min(min_dim, rank)
-
-    # make covariance matrices
-    CXX = (X.T @ X + lam * torch.eye(X.shape[1], device=X.device)) / X.shape[0]
-    CYX = (Y.T @ X) / X.shape[0]
-
-    # compute inverse square root of matrix
-    # s, u = eigh(CXX.cpu().numpy())
-    u, s = torch.svd_lowrank(CXX, q=rank)[:2]
-    CXXMH = (u * (s + lam) ** -0.5) @ u.T
-
-    # project into prediction space
-    M = CYX @ CXXMH
-    # do svd of prediction projection
-    # model = PCA(n_components=rank).fit(M)
-    # c = model.components_.T
-    # s = model.singular_values_
-    s, c = torch.svd_lowrank(M, q=rank)[1:]
-    A = M @ c
-    B = CXXMH @ c
-    return A, B
-
-
-def linear_prediction(X, Y, rank=None, lam=0, allranks=True, itrain=None, itest=None, tbin=None, device=torch.device("cuda")):
-    """predict Y from X using regularized regression
-    *** user needs to subtract mean from X and Y before predicting ***
-    
-    if rank is None, performs ridge regression, otherwise performs reduced rank regression
-    
-    Prediction:
-    >>> Y_pred_test = X_test @ B @ A.T
-    Parameters
-    ----------
-    X : 2D array, input data, float32 (n_samples, n_features)
-    Y : 2D array, data to predict, float32 (n_samples, n_predictors)
-    rank : int (optional, default None)
-        rank up to which to compute reduced rank regression for
-    lam : float (optional, default 0)
-        regularizer
-    allranks : bool (optional, default True)
-        compute variance explained at all ranks
-    itrain: 1D int array (optional, default None)
-        times in train set
-    itest: 1D int array (optional, default None)
-        times in test set
-    tbin: int (optional, default None)
-        also compute variance explained in bins of tbin
-    Returns
-    --------
-    Y_pred_test : 2D array - prediction of Y with max rank (len(itest), n_features)
-    varexp : 1D array - variance explained across all features (rank,)
-    itest: 1D int array
-        times in test set
-    A : 2D array - prediction matrix 1 (n_predictors, rank)
-    B : 2D array - prediction matrix 2 (n_features, rank)
-    varexpf : 1D array - variance explained per feature (rank, n_features)
-    corrf : 1D array - correlation with Y per feature (rank, n_features)
-
-    """
-    n_t, n_feats = Y.shape
-    if itrain is None and itest is None:
-        itrain, itest = split_traintest(n_t)
-    itrain, itest = itrain.flatten(), itest.flatten()
-    X = torch.from_numpy(X).to(device)
-    Y = torch.from_numpy(Y).to(device)
-    if rank is not None:
-        min_dim = min(Y.shape[1], min(X.shape[0], X.shape[1])) - 1
-        rank = min(min_dim, rank)
-        A, B = reduced_rank_regression(
-            X[itrain], Y[itrain], rank=rank, lam=lam
-        )
-    else:
-        A = ridge_regression(X[itrain], Y[itrain], lam=lam)
-        B = None
-        allranks = False
-
-    corrf = np.zeros((rank, n_feats))
-    varexpf = np.zeros((rank, n_feats))
-    varexp = np.zeros((rank, 2)) if (tbin is not None and tbin > 1) else np.zeros((rank, 1))
-    Y_pred_test = np.zeros((len(itest), n_feats))
-    for r in range(0 if allranks else rank-1, rank):
-        if B is not None:
-            Y_pred_test = X[itest] @ B[:, : r + 1] @ A[:, : r + 1].T
-        else:
-            Y_pred_test = X[itest] @ A.T
-        Y_test_var = (Y[itest] ** 2).mean(axis=0)
-        corrf[r] = ((Y[itest] * Y_pred_test).mean(axis=0) / 
-                    (Y_test_var ** 0.5 * Y_pred_test.std(axis=0))).cpu().numpy()
-        residual = ((Y[itest] - Y_pred_test) ** 2).mean(axis=0)
-        varexpf[r] = (1 - residual / Y_test_var).cpu().numpy()
-        varexp[r, 0] = (1 - residual.mean() / Y_test_var.mean()).cpu().numpy()
-        if tbin is not None and tbin > 1:
-            varexp[r, 1] = compute_varexp(bin1d(Y[itest], tbin).flatten(), bin1d(Y_pred_test, tbin).flatten()).cpu().numpy()
-    if not allranks:
-        varexp, varexpf, corrf = varexp[-1:], varexpf[-1:], corrf[-1:]
-    return (Y_pred_test.cpu().numpy(), varexp.squeeze(), itest, 
-            A.cpu().numpy(), B.cpu().numpy(), varexpf.squeeze(), corrf.squeeze())
-
-def prediction_wrapper(X, Y, tcam=None, tneural=None, U=None, spks=None, delay=0, tbin=None, rank=32):
-    """ predict neurons or neural PCs Y and compute varexp for Y and/or spks"""
-    
-    X -= X.mean(axis=0)
-    X /= X[:,0].std(axis=0)
-
-    if tcam is not None and tneural is not None:
-        X_ds = resample_data(X, tcam, tneural, crop='linspace')
-
-    if delay < 0:
-        Ys = np.vstack((Y[-delay:], np.tile(Y[[-1],:], (-delay,1))))
-    else:
-        X_ds = np.vstack((X_ds[delay:], np.tile(X_ds[[-1],:], (delay,1))))
-        Ys = Y
-    
-    Y_pred_test, ve_test, itest, A, B = linear_prediction(X_ds, Ys, rank=rank, lam=1e-6, tbin=tbin)[:5]
-    varexp = ve_test
-    # return Y_pred_test at specified rank
-    Y_pred_test = X_ds[itest] @ B[:,:rank] @ A[:,:rank].T
-
-    # single neuron prediction
-    if U is not None and spks is not None:
-        spks_pred_test = Y_pred_test @ U.T 
-        spks_test = spks[:, itest-delay].T
-        varexp_neurons = np.nan * np.zeros((len(spks), 2 if tbin is not None and tbin>1 else 1))
-        varexp_neurons[:,0] = compute_varexp(spks_test, spks_pred_test)
-        if tbin is not None and tbin > 1:
-            spks_test_bin = bin1d(spks_test, tbin)
-            spks_pred_test_bin = bin1d(spks_pred_test, tbin)
-            varexp_neurons[:,1] = compute_varexp(spks_test_bin, spks_pred_test_bin)
-        spks_pred_test0 = spks_pred_test.copy()
-        
-        return varexp.squeeze(), varexp_neurons.squeeze(), spks_pred_test0, itest
-    else:
-        return varexp.squeeze(), None, None, itest
-
-
-def CCA(x1, x2, lam=1):
-    from sklearn.decomposition import TruncatedSVD as SVD
-    n_comp = np.min(x1.shape)-1
-    model1 = SVD(n_components = min(1000, n_comp)).fit(x1)
-    n_comp = np.min(x2.shape)-1
-    model2 = SVD(n_components = min(1000, x2.shape[1]-1)).fit(x2)
-
-    U0 = model1.components_
-    V0 = U0 @ x1.T
-
-    print(U0.shape, V0.shape)
-
-    U1 = model2.components_
-    V1 = U1 @ x2.T
-
-    S0 = np.sum(V0**2, axis=1)**.5
-    V0 = V0/S0[:, np.newaxis]
-
-    S1 = np.sum(V1**2, axis=1)**.5
-    V1 = V1/S1[:, np.newaxis]
-
-    lam = lam * x1.shape[-1]
-
-    VVT = V0 @ V1.T
-    W0 = U0.T * S0/(S0**2 + lam)**.5
-    W1 = U1.T * S1/(S1**2 + lam)**.5
-
-    CC = W0 @ (VVT @ W1.T)
-    CC = CC + CC.T
-
-    model3 = SVD(n_components = min(100, CC.shape[0]-1)).fit(CC)
-
-    u = model3.components_
-    print(u.shape)
-    v = u @ CC.T
-    v = v / np.sum(v**2, axis=1)[:, np.newaxis]**.5
-    u = u @ (U0.T /(S0**2 + lam)**.5) @ U0
-    v = v @ (U1.T /(S1**2 + lam)**.5) @ U1
-
+"""
+Copright © 2023 Howard Hughes Medical Institute, Authored by Carsen Stringer and Marius Pachitariu.
+"""
+import numpy as np 
+import torch
+
+from neuropop.utils import compute_varexp, bin1d, resample_data
+from neuropop.split_data import split_traintest
+
+
+def ridge_regression(X, Y, lam=0):
+    """predict Y from X using regularized linear regression using torch arrays
+    *** subtract mean from X and Y before predicting
+    Prediction:
+    >>> Y_pred = X @ A
+    Parameters
+    ----------
+    X : 2D array, input data (n_samples, n_features)
+    Y : 2D array, data to predict (n_samples, n_predictors)
+    Returns
+    --------
+    A : 2D array - prediction matrix 1 (n_predictors, rank)
+    """
+    if torch.is_tensor(X):
+        eyem = torch.eye(X.shape[1], dtype=torch.float, device=X.device)
+        solve = torch.linalg.solve
+    else:
+        eyem = np.eye(X.shape[1], dtype=X.dtype)
+        solve = np.linalg.solve
+    CXX = (X.T @ X + lam * eyem) / X.shape[0]
+    CXY = (X.T @ Y) / X.shape[0]
+    A = solve(CXX, CXY).T
+    return A
+
+def reduced_rank_regression(X, Y, rank=None, lam=0):
+    """predict Y from X using regularized reduced rank regression using torch arrays
+    *** subtract mean from X and Y before predicting
+    if rank is None, returns A and B of full-rank (minus one) prediction
+    Prediction:
+    >>> Y_pred = X @ B @ A.T
+    Parameters
+    ----------
+    X : 2D array, input data, float32 torch tensor (n_samples, n_features)
+    Y : 2D array, data to predict, float32 torch tensor (n_samples, n_predictors)
+    rank : int (optional, default None)
+        rank to compute reduced rank regression for
+    lam : float (optional, default 0)
+        regularizer
+    Returns
+    --------
+    A : 2D array - prediction matrix 1 (n_predictors, rank)
+    B : 2D array - prediction matrix 2 (n_features, rank)
+    """
+    min_dim = min(Y.shape[1], min(X.shape[0], X.shape[1])) - 1
+    if rank is None:
+        rank = min_dim
+    else:
+        rank = min(min_dim, rank)
+
+    # make covariance matrices
+    CXX = (X.T @ X + lam * torch.eye(X.shape[1], device=X.device)) / X.shape[0]
+    CYX = (Y.T @ X) / X.shape[0]
+
+    # compute inverse square root of matrix
+    # s, u = eigh(CXX.cpu().numpy())
+    u, s = torch.svd_lowrank(CXX, q=rank)[:2]
+    CXXMH = (u * (s + lam) ** -0.5) @ u.T
+
+    # project into prediction space
+    M = CYX @ CXXMH
+    # do svd of prediction projection
+    # model = PCA(n_components=rank).fit(M)
+    # c = model.components_.T
+    # s = model.singular_values_
+    s, c = torch.svd_lowrank(M, q=rank)[1:]
+    A = M @ c
+    B = CXXMH @ c
+    return A, B
+
+
+def linear_prediction(X, Y, rank=None, lam=0, allranks=True, itrain=None, itest=None, tbin=None, device=torch.device("cpu")):
+    """predict Y from X using regularized regression
+    *** user needs to subtract mean from X and Y before predicting ***
+    
+    if rank is None, performs ridge regression, otherwise performs reduced rank regression
+    
+    Prediction:
+    >>> Y_pred_test = X_test @ B @ A.T
+    Parameters
+    ----------
+    X : 2D array, input data, float32 (n_samples, n_features)
+    Y : 2D array, data to predict, float32 (n_samples, n_predictors)
+    rank : int (optional, default None)
+        rank up to which to compute reduced rank regression for
+    lam : float (optional, default 0)
+        regularizer
+    allranks : bool (optional, default True)
+        compute variance explained at all ranks
+    itrain: 1D int array (optional, default None)
+        times in train set
+    itest: 1D int array (optional, default None)
+        times in test set
+    tbin: int (optional, default None)
+        also compute variance explained in bins of tbin
+    Returns
+    --------
+    Y_pred_test : 2D array - prediction of Y with max rank (len(itest), n_features)
+    varexp : 1D array - variance explained across all features (rank,)
+    itest: 1D int array
+        times in test set
+    A : 2D array - prediction matrix 1 (n_predictors, rank)
+    B : 2D array - prediction matrix 2 (n_features, rank)
+    varexpf : 1D array - variance explained per feature (rank, n_features)
+    corrf : 1D array - correlation with Y per feature (rank, n_features)
+
+    """
+    n_t, n_feats = Y.shape
+    if itrain is None and itest is None:
+        itrain, itest = split_traintest(n_t)
+    itrain, itest = itrain.flatten(), itest.flatten()
+    X = torch.from_numpy(X).float().to(device)
+    Y = torch.from_numpy(Y).float().to(device)
+    if rank is not None:
+        min_dim = min(Y.shape[1], min(X.shape[0], X.shape[1])) - 1
+        rank = min(min_dim, rank)
+        A, B = reduced_rank_regression(
+            X[itrain], Y[itrain], rank=rank, lam=lam
+        )
+    else:
+        A = ridge_regression(X[itrain], Y[itrain], lam=lam)
+        B = None
+        allranks = False
+        rank = 1
+
+    corrf = np.zeros((rank, n_feats))
+    varexpf = np.zeros((rank, n_feats))
+    varexp = np.zeros((rank, 2)) if (tbin is not None and tbin > 1) else np.zeros((rank, 1))
+    Y_pred_test = np.zeros((len(itest), n_feats))
+    for r in range(0 if allranks else rank-1, rank):
+        if B is not None:
+            Y_pred_test = X[itest] @ B[:, : r + 1] @ A[:, : r + 1].T
+        else:
+            Y_pred_test = X[itest] @ A.T
+        Y_test_var = (Y[itest] ** 2).mean(axis=0)
+        corrf[r] = ((Y[itest] * Y_pred_test).mean(axis=0) / 
+                    (Y_test_var ** 0.5 * Y_pred_test.std(axis=0))).cpu().numpy()
+        residual = ((Y[itest] - Y_pred_test) ** 2).mean(axis=0)
+        varexpf[r] = (1 - residual / Y_test_var).cpu().numpy()
+        varexp[r, 0] = (1 - residual.mean() / Y_test_var.mean()).cpu().numpy()
+        if tbin is not None and tbin > 1:
+            varexp[r, 1] = compute_varexp(bin1d(Y[itest], tbin).flatten(), bin1d(Y_pred_test, tbin).flatten()).cpu().numpy()
+    if not allranks:
+        varexp, varexpf, corrf = varexp[-1:], varexpf[-1:], corrf[-1:]
+    if B is not None:
+        B = B.cpu().numpy()
+    return (Y_pred_test.cpu().numpy(), varexp.squeeze(), itest, 
+            A.cpu().numpy(), B, varexpf.squeeze(), corrf.squeeze())
+
+def prediction_wrapper(X, Y, tcam=None, tneural=None, U=None, spks=None, 
+                    delay=0, tbin=None, rank=None, lam=0, device=torch.device('cuda')):
+    """ predict neurons or neural PCs Y and compute varexp for Y and/or spks"""
+    
+    X -= X.mean(axis=0)
+    X /= X[:,0].std(axis=0)
+
+    if tcam is not None and tneural is not None:
+        X_ds = resample_data(X, tcam, tneural, crop='linspace')
+    else:
+        X_ds = X
+
+    if delay < 0:
+        Ys = np.vstack((Y[-delay:], np.tile(Y[[-1],:], (-delay,1))))
+    else:
+        X_ds = np.vstack((X_ds[delay:], np.tile(X_ds[[-1],:], (delay,1))))
+        Ys = Y
+    
+    Y_pred_test, ve_test, itest, A, B = linear_prediction(X_ds, Ys, rank=rank, 
+                                                    lam=lam, tbin=tbin, device=device)[:5]
+    varexp = ve_test
+    # return Y_pred_test at specified rank
+    if B is not None:
+        Y_pred_test = X[itest] @ B[:, :rank] @ A[:, :rank].T
+    else:
+        Y_pred_test = X[itest] @ A.T
+    
+    # single neuron prediction
+    if U is not None and spks is not None:
+        spks_pred_test = Y_pred_test @ U.T 
+        spks_test = spks[:, itest-delay].T
+        varexp_neurons = np.nan * np.zeros((len(spks), 2 if tbin is not None and tbin>1 else 1))
+        varexp_neurons[:,0] = compute_varexp(spks_test, spks_pred_test)
+        if tbin is not None and tbin > 1:
+            spks_test_bin = bin1d(spks_test, tbin)
+            spks_pred_test_bin = bin1d(spks_pred_test, tbin)
+            varexp_neurons[:,1] = compute_varexp(spks_test_bin, spks_pred_test_bin)
+        spks_pred_test0 = spks_pred_test.copy()
+        
+        return varexp.squeeze(), varexp_neurons.squeeze(), spks_pred_test0, itest
+    else:
+        return varexp.squeeze(), None, Y_pred_test, itest
+
+
+def CCA(x1, x2, lam=1):
+    from sklearn.decomposition import TruncatedSVD as SVD
+    n_comp = np.min(x1.shape)-1
+    model1 = SVD(n_components = min(1000, n_comp)).fit(x1)
+    n_comp = np.min(x2.shape)-1
+    model2 = SVD(n_components = min(1000, x2.shape[1]-1)).fit(x2)
+
+    U0 = model1.components_
+    V0 = U0 @ x1.T
+
+    print(U0.shape, V0.shape)
+
+    U1 = model2.components_
+    V1 = U1 @ x2.T
+
+    S0 = np.sum(V0**2, axis=1)**.5
+    V0 = V0/S0[:, np.newaxis]
+
+    S1 = np.sum(V1**2, axis=1)**.5
+    V1 = V1/S1[:, np.newaxis]
+
+    lam = lam * x1.shape[-1]
+
+    VVT = V0 @ V1.T
+    W0 = U0.T * S0/(S0**2 + lam)**.5
+    W1 = U1.T * S1/(S1**2 + lam)**.5
+
+    CC = W0 @ (VVT @ W1.T)
+    CC = CC + CC.T
+
+    model3 = SVD(n_components = min(100, CC.shape[0]-1)).fit(CC)
+
+    u = model3.components_
+    print(u.shape)
+    v = u @ CC.T
+    v = v / np.sum(v**2, axis=1)[:, np.newaxis]**.5
+    u = u @ (U0.T /(S0**2 + lam)**.5) @ U0
+    v = v @ (U1.T /(S1**2 + lam)**.5) @ U1
+
     return u,v
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `neuropop-0.1/neuropop/nn_prediction.py` & `neuropop-1.0/neuropop/nn_prediction.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,370 +1,421 @@
-import sys, time
-import numpy as np
-import torch
-from torch import nn
-from torch.nn import functional as F
-
-from neuropop.filtering import gabor_wavelet
-from neuropop.utils import bin1d, compute_varexp
-from neuropop.split_data import split_data
-
-def network_wrapper(x, Y, tcam, tneural, U, spks, delay=-1,
-                        verbose=False, per_pt=False, device=torch.device('cuda')):
-    x = (x - x.mean(axis=0)) / x[:,0].std(axis=0)
-    
-    np.random.seed(0); torch.manual_seed(0); torch.cuda.manual_seed(0)
-    model = PredictionNetwork(n_in=x.shape[-1], n_out=Y.shape[-1]).to(device)
-
-    y_pred_test, ve_test, itest = model.train_model(x, Y, tcam, tneural, delay=delay, 
-                                                verbose=verbose, device=device)
-                                                
-    y_pred_test = y_pred_test.reshape(-1, Y.shape[-1])
-    varexp = np.zeros(2)
-    varexp_neurons = np.zeros((len(spks), 2))
-    varexp[0] = ve_test
-    Y_test_bin = bin1d(Y[itest.flatten()], 4)
-    Y_pred_test_bin = bin1d(y_pred_test, 4)
-    varexp[1] = 1 - ((Y_test_bin - Y_pred_test_bin)**2).mean() / ((Y_test_bin)**2).mean()
-    print(f'all kp, varexp {varexp[0]:.3f}; tbin=4: {varexp[1]:.3f}')
-    spks_pred_test = y_pred_test @ U.T
-    spks_test = spks[:,itest.flatten()].T
-    varexp_neurons[:,0] = compute_varexp(spks_test, spks_pred_test)
-    spks_test_bin = bin1d(spks_test, 4)
-    spks_pred_test_bin = bin1d(spks_pred_test, 4)
-    varexp_neurons[:,1] = compute_varexp(spks_test_bin, spks_pred_test_bin)
-    spks_pred_test0 = spks_pred_test.T.copy()
-
-    # predict using each variable
-    if per_pt:
-        varexp_per_pt = np.nan * np.zeros((x.shape[1], 2))
-        varexp_neurons_per_pt = np.nan * np.zeros((len(spks), x.shape[1], 2))
-        for k in enumerate(x.shape[1]):
-            np.random.seed(0); torch.manual_seed(0); torch.cuda.manual_seed(0)
-            model = PredictionNetwork(n_in=1, n_out=Y.shape[-1]).to(device)
-
-            y_pred_test, ve_test, itest = model.train_model(x[:, k],
-                                                        Y, tcam, tneural, 
-                                                      delay=delay, device=device)
-            y_pred_test = y_pred_test.reshape(-1, Y.shape[-1])
-            varexp_per_pt[k,0] = ve_test      
-            varexp_per_pt[k,1] = compute_varexp(bin1d(Y[itest.flatten()], 4).flatten(), 
-                                                bin1d(y_pred_test, 4).flatten())
-            spks_pred_test = y_pred_test @ U.T
-            spks_test = spks[:,itest.flatten()].T
-            varexp_neurons_per_pt[:,k,0] = compute_varexp(spks_test, spks_pred_test)
-            spks_test_bin = bin1d(spks_test, 4)
-            spks_pred_test_bin = bin1d(spks_pred_test, 4)
-            varexp_neurons_per_pt[:,k,1] = compute_varexp(spks_test_bin, spks_pred_test_bin)
-            print(f'{k}, varexp {ve_test:.3f}, {varexp_neurons_per_pt[:,k,0].mean():.3f}')
-            return varexp, varexp_neurons, spks_pred_test0, itest, varexp_per_pt, varexp_neurons_per_pt
-    else:
-        return varexp, varexp_neurons, spks_pred_test0, itest, model
-
-class Core(nn.Module):
-    """ linear -> conv1d -> relu -> linear -> relu = latents for KPN model"""
-    def __init__(self, n_in=28, n_kp=None, n_filt=10, kernel_size=201, 
-                 n_layers=1, n_med=50, n_latents=256, 
-                 identity=False, same_conv=True, 
-                 relu_wavelets=True, relu_latents=True):
-        super().__init__()
-        self.n_in = n_in
-        self.n_kp = n_in if n_kp is None or identity else n_kp
-        self.n_filt = (n_filt//2) * 2 # must be even for initialization
-        self.relu_latents = relu_latents
-        self.relu_wavelets = relu_wavelets
-        self.same_conv = same_conv
-        self.n_layers = n_layers
-        self.n_latents = n_latents
-        self.features = nn.Sequential()
-
-        # combine keypoints into n_kp features
-        if identity:
-            self.features.add_module('linear0', nn.Identity(self.n_in))
-        else:
-            self.features.add_module('linear0', nn.Sequential(nn.Linear(self.n_in, self.n_kp),
-                                                              ))
-        # initialize filters with gabors
-        f = np.geomspace(1, 10, self.n_filt//2).astype('float32')
-        gw0 = gabor_wavelet(1, f[:,np.newaxis], 0, n_pts=kernel_size)
-        gw1 = gabor_wavelet(1, f[:,np.newaxis], np.pi/2, n_pts=kernel_size)
-        if self.same_conv:
-            # compute n_filt wavelet features of each one => n_filt * n_kp features
-            self.features.add_module('wavelet0', nn.Conv1d(1, self.n_filt, kernel_size=kernel_size,
-                                                        padding=kernel_size//2, bias=False))
-            self.features[-1].weight.data = torch.from_numpy(np.vstack((gw0, gw1))).unsqueeze(1)
-        else:
-            self.features.add_module('wavelet0', nn.Conv1d(self.n_kp, self.n_kp, kernel_size=kernel_size,
-                                                        padding=kernel_size//2, bias=False, groups=self.n_kp))
-            self.features[-1].weight.data = torch.tile(torch.from_numpy(gw0[[1]]).unsqueeze(1), 
-                                                        (self.n_kp, 1, 1))
-            self.n_filt = 1
-        for n in range(1, n_layers):
-            n_in = self.n_kp * self.n_filt if n==1 else n_med
-            self.features.add_module(f'linear{n}', nn.Sequential(nn.Linear(n_in, 
-                                                                            n_med),
-                                                                 ))
-
-        # latent linear layer
-        n_med = n_med if n_layers > 1 else self.n_filt * self.n_kp
-        self.features.add_module('latent', nn.Sequential(nn.Linear(n_med, n_latents),
-                                                        ))
-        
-    def wavelets(self, x):
-        """ compute wavelets of keypoints through linear + conv1d + relu layer """
-        # x is (n_batches, time, features)
-        out = self.features[0](x.reshape(-1, x.shape[-1]))
-        out = out.reshape(x.shape[0], x.shape[1], -1).transpose(2,1)
-        # out is now (n_batches, n_kp, time)
-        if self.same_conv:
-            out = out.reshape(-1, out.shape[-1]).unsqueeze(1)
-            # out is now (n_batches * n_kp, 1, time)
-            out = self.features[1](out)
-            # out is now (n_batches * n_kp, n_filt, time)
-            out = out.reshape(-1, self.n_kp * self.n_filt, out.shape[-1]).transpose(2,1)
-            out = out.reshape(-1, self.n_kp * self.n_filt)
-        else:
-            out = self.features[1](out)
-            out = out.transpose(-1,-2)
-        if self.relu_wavelets:
-            out = F.relu(out)
-        
-        # if n_layers > 1, go through more linear layers
-        for n in range(1, self.n_layers):
-            out = self.features[n+1](out)
-            out = F.relu(out)
-        return out
-                                              
-    def forward(self, x=None, wavelets=None):
-        """ x is (n_batches, time, features)
-            sample_inds is (sub_time) over batches
-        """
-        if wavelets is None:
-            wavelets = self.wavelets(x)
-        wavelets = wavelets.reshape(-1, wavelets.shape[-1])
-        
-        # latent layer
-        latents = self.features[-1](wavelets)
-        latents = latents.reshape(x.shape[0], -1, latents.shape[-1])
-        if self.relu_latents:
-            latents = F.relu(latents)
-        latents = latents.reshape(-1, latents.shape[-1])
-        return latents
-
-class Readout(nn.Module):
-    """ linear layer from latents to neural PCs or neurons """
-    def __init__(self, n_animals=1, n_latents=256, n_layers=1, 
-                n_med=128, n_out=128):
-        super().__init__()
-        self.n_animals = n_animals
-        self.linear = nn.Sequential()
-        self.bias = nn.Parameter(torch.zeros(n_out))
-        if n_animals==1:
-            for j in range(n_layers):
-                n_in = n_latents if j==0 else n_med 
-                n_outc = n_out if j==n_layers-1 else n_med 
-                self.linear.append(nn.Linear(n_in, n_outc))
-                if n_layers > 1 and j < n_layers-1:
-                    self.linear.append(nn.ReLU())
-        else:
-            # no option for n_layers > 1
-            for n in range(n_animals):
-                self.linear.append(nn.Linear(n_latents, n_out))
-        self.bias.requires_grad = False
-
-    def forward(self, latents, animal_id=0):
-        if self.n_animals==1:
-            return self.linear(latents) + self.bias
-        else:
-            return self.linear[animal_id](latents) + self.bias
-
-class PredictionNetwork(nn.Module):
-    """ predict from behavior to neural PCs / neural activity model """
-    def __init__(self, n_in=28, n_kp=None, n_filt=10, kernel_size=201, n_core_layers=2,
-                 n_latents=256, n_out_layers=1, n_out=128, n_med=50, n_animals=1, same_conv=True,
-                 identity=False, relu_wavelets=True, relu_latents=True):
-        super().__init__()
-        self.core = Core(n_in=n_in, n_kp=n_kp, n_filt=n_filt, kernel_size=kernel_size, 
-                         n_layers=n_core_layers, n_med=n_med, n_latents=n_latents, same_conv=same_conv,
-                         identity=identity, relu_wavelets=relu_wavelets, relu_latents=relu_latents)
-        self.readout = Readout(n_animals=n_animals, n_latents=n_latents, n_layers=n_out_layers, 
-                                n_out=n_out)
-
-    def forward(self, x, sample_inds=None, animal_id=0):
-        latents = self.core(x)
-        if sample_inds is not None:
-            latents = latents[sample_inds]
-        latents = latents.reshape(x.shape[0], -1, latents.shape[-1])
-        y_pred = self.readout(latents, animal_id=animal_id)
-        return y_pred, latents
-    
-    def train_model(self, X_dat, Y_dat, tcam_list, tneural_list, 
-                        delay=-1, smoothing_penalty=0.5, 
-                    n_iter=300, learning_rate=5e-4, annealing_steps=2,
-                    weight_decay=1e-4, device=torch.device('cuda'), 
-                    split_time=False, verbose=False):
-        """ train behavior -> neural model using multiple animals """
-
-        optimizer = torch.optim.AdamW(self.parameters(), lr=learning_rate, weight_decay=weight_decay)
-        ### make input data a list if it's not already
-        not_list = False
-        if not isinstance(X_dat, list):
-            not_list = True
-            X_dat, Y_dat, tcam_list, tneural_list = [X_dat], [Y_dat], [tcam_list], [tneural_list]
-        
-        ### split data into train / test and concatenate
-        arrs = [[],[],[],[],[],[],[],[],[],[]]
-        for i, (X, Y, tcam, tneural) in enumerate(zip(X_dat, Y_dat, tcam_list, tneural_list)):
-            dsplits = split_data(X, Y, tcam, tneural, delay=delay, split_time=split_time, device=device)
-            for d,a in zip(dsplits, arrs):
-                a.append(d)
-        X_train, X_test, Y_train, Y_test, itrain_sample_b, itest_sample_b, itrain_sample, itest_sample, itrain, itest = arrs
-        n_animals = len(X_train)
-        
-        tic = time.time()
-        ### determine total number of batches across all animals to sample from
-        n_batches = [0]
-        n_batches.extend([X_train[i].shape[0] for i in range(n_animals)]) 
-        n_batches = np.array(n_batches)
-        c_batches = np.cumsum(n_batches)
-        n_batches = n_batches.sum()   
-
-        anneal_epochs = n_iter - 50*np.arange(1, annealing_steps+1)
-
-        ### optimize all parameters with SGD
-        for epoch in range(n_iter):
-            self.train()
-            if epoch in anneal_epochs:
-                if verbose:
-                    print('annealing learning rate')
-                optimizer.param_groups[0]['lr'] /= 10.
-            np.random.seed(epoch)
-            rperm = np.random.permutation(n_batches)
-            train_loss = 0
-            for nr in rperm:
-                i = np.nonzero(nr >= c_batches)[0][-1]
-                n = nr - c_batches[i]
-                y_pred = self.forward(X_train[i][n].unsqueeze(0), 
-                            itrain_sample_b[i][n], 
-                            animal_id=i)[0]
-                loss = ((y_pred - Y_train[i][n].unsqueeze(0))**2).mean()
-                loss += smoothing_penalty * (torch.diff(self.core.features[1].weight)**2).sum()
-                optimizer.zero_grad()
-                loss.backward()
-                optimizer.step()
-                train_loss += loss.item()
-                
-            train_loss /= n_batches
-
-            # compute test loss and test variance explained
-            if epoch%20==0 or epoch==n_iter-1:
-                ve_all, y_pred_all = [], []
-                self.eval()
-                with torch.no_grad():
-                    pstr = f'epoch {epoch}, '
-                    for i in range(n_animals):
-                        y_pred = self.forward(X_test[i], itest_sample_b[i].flatten(), animal_id=i)[0]
-                        y_pred = y_pred.reshape(-1, y_pred.shape[-1])
-                        tl = ((y_pred - Y_test[i])**2).mean()
-                        ve = 1 - tl / ((Y_test[i] - Y_test[i].mean(axis=0))**2).mean()
-                        y_pred_all.append(y_pred.cpu().numpy())
-                        ve_all.append(ve.item())
-                        if n_animals==1:
-                            pstr += f'animal {i}, train loss {train_loss:.4f}, test loss {tl.item():.4f}, varexp {ve.item():.4f}, '
-                        else:
-                            pstr += f'varexp{i} {ve.item():.4f}, '
-                pstr += f'time {time.time()-tic:.1f}s'
-                if verbose:
-                    print(pstr)
-        
-        if not_list:
-            return y_pred_all[0], ve_all[0], itest[0]
-        else:
-            return y_pred_all, ve_all, itest
-
-def train_model_test(model, X, Y, tcam, tneural, sgd=False, lam=1e-3, 
-                   n_iter=600, learning_rate=5e-4, fix_model=True,
-                   smoothing_penalty=1.0,
-                   weight_decay=1e-4, device=torch.device('cuda')):
-
-    dsplits = split_data(X, Y, tcam, tneural, device=device)
-    X_train, X_test, Y_train, Y_test, itrain_sample_b, itest_sample_b, itrain_sample, itest_sample, itrain, itest = dsplits
-            
-    tic = time.time()
-
-    n_batches = X_train.shape[0]
-    if sgd:
-        model.train()
-        if fix_model:
-            for param in model.parameters():
-                param.requires_grad = False 
-            model.test_classifier.weight.requires_grad = True
-            model.test_classifier.bias.requires_grad = True
-        else:
-            for param in model.parameters():
-                param.requires_grad = True 
-            
-        
-        optimizer = torch.optim.AdamW(model.parameters(), lr=learning_rate, weight_decay=weight_decay)
-        for epoch in range(n_iter):
-            model.train()
-            np.random.seed(epoch)
-            rperm = np.random.permutation(n_batches)
-            train_loss = 0
-            for n in rperm:
-                y_pred, latents = model(X_train[n].unsqueeze(0), 
-                                    itrain_sample_b[n], 
-                                    test=True)
-                loss = ((y_pred - Y_train[n].unsqueeze(0))**2).mean()
-                loss += smoothing_penalty * (torch.diff(model.features[1].weight)**2).sum()
-                optimizer.zero_grad()
-                loss.backward()
-                optimizer.step()
-                train_loss += loss.item()
-            train_loss /= n_batches
-            if epoch%20==0 or epoch==n_iter-1:
-                ve_all = []
-                y_pred_all = []
-                with torch.no_grad():
-                    model.eval()
-                    pstr = f'epoch {epoch}, '
-                    y_pred = model(X_test, itest_sample_b.flatten(), test=True)[0]
-                    tl = ((y_pred - Y_test)**2).mean()
-                    ve = 1 - tl / (Y_test**2).mean()
-                    #ve = ve.item()
-                    y_pred = y_pred.cpu().numpy()
-                    #y_pred_all.append(y_pred.cpu().numpy())
-                    #ve_all.append(ve.item())
-                    pstr += f'train loss {train_loss:.4f}, test loss {tl.item():.4f}, varexp {ve.item():.4f}'
-                    print(pstr)
-
-    else:
-        itrain = itrain.reshape(n_batches, -1)
-        l_train = itrain.shape[-1]
-        with torch.no_grad():
-            model.eval()
-            for n in range(n_batches):
-                y_pred, latents = model(X_train[n].unsqueeze(0), 
-                                    itrain_sample_b[n], 
-                                    test=True)
-                if n==0:
-                    n_latents = latents.shape[-1]
-                    latents_train = np.ones((itrain.size, n_latents+1), 'float32')
-                latents_train[n*l_train : (n+1)*l_train, :n_latents] = latents.cpu().numpy()
-            latents_test = np.ones((itest.size, n_latents+1), 'float32')
-            latents_test[:,:n_latents] = model(X_test, 
-                                            itest_sample_b.flatten(), 
-                                            test=True)[1].cpu().numpy().reshape(-1, n_latents)
-
-            Y_train = Y_train.cpu().numpy()
-            Y_test = Y_test.cpu().numpy().reshape(-1, Y_test.shape[-1])
-            Y_train = Y_train.reshape(-1, Y_train.shape[-1])          
-            A = np.linalg.solve(latents_train.T @ latents_train + lam * np.eye(n_latents+1),
-                                latents_train.T @ Y_train)
-            y_pred = latents_test @ A 
-            tl = ((y_pred - Y_test)**2).mean()
-            ve = 1 - tl / (Y_test**2).mean()
-            model.test_classifier.weight.data = torch.from_numpy(A[:n_latents].T).float().to(device)
-            model.test_classifier.bias.data = torch.from_numpy(A[-1]).float().to(device)
-            print(ve)
-
-    return y_pred, ve, itest
+"""
+Copright © 2023 Howard Hughes Medical Institute, Authored by Carsen Stringer and Marius Pachitariu.
+"""
+import sys, time
+import numpy as np
+import torch
+from torch import nn
+from torch.nn import functional as F
+
+from neuropop.filtering import gabor_wavelet
+from neuropop.utils import bin1d, compute_varexp
+from neuropop.split_data import split_data
+
+def network_wrapper(x, Y, tcam, tneural, spks, U, delay=-1,
+                        verbose=False, per_pt=False, device=torch.device('cuda')):
+    x = (x - x.mean(axis=0)) / x[:,0].std(axis=0)
+    
+    np.random.seed(0); torch.manual_seed(0); torch.cuda.manual_seed(0)
+    model = PredictionNetwork(n_in=x.shape[-1], n_out=Y.shape[-1]).to(device)
+
+    y_pred_test, ve_test, itest = model.train_model(x, Y, tcam, tneural, delay=delay, 
+                                                verbose=verbose, device=device)
+                                                
+    y_pred_test = y_pred_test.reshape(-1, Y.shape[-1])
+    varexp = np.zeros(2)
+    varexp_neurons = np.zeros((len(spks), 2))
+    varexp[0] = ve_test
+    Y_test_bin = bin1d(Y[itest.flatten()], 4)
+    Y_pred_test_bin = bin1d(y_pred_test, 4)
+    varexp[1] = 1 - ((Y_test_bin - Y_pred_test_bin)**2).mean() / ((Y_test_bin)**2).mean()
+    print(f'all kp, varexp {varexp[0]:.3f}; tbin=4: {varexp[1]:.3f}')
+    spks_pred_test = y_pred_test @ U.T
+    spks_test = spks[:,itest.flatten()].T
+    varexp_neurons[:,0] = compute_varexp(spks_test, spks_pred_test)
+    spks_test_bin = bin1d(spks_test, 4)
+    spks_pred_test_bin = bin1d(spks_pred_test, 4)
+    varexp_neurons[:,1] = compute_varexp(spks_test_bin, spks_pred_test_bin)
+    spks_pred_test0 = spks_pred_test.T.copy()
+
+    # predict using each variable
+    if per_pt:
+        varexp_per_pt = np.nan * np.zeros((x.shape[1], 2))
+        varexp_neurons_per_pt = np.nan * np.zeros((len(spks), x.shape[1], 2))
+        for k in enumerate(x.shape[1]):
+            np.random.seed(0); torch.manual_seed(0); torch.cuda.manual_seed(0)
+            model = PredictionNetwork(n_in=1, n_out=Y.shape[-1]).to(device)
+
+            y_pred_test, ve_test, itest = model.train_model(x[:, k],
+                                                        Y, tcam, tneural, 
+                                                      delay=delay, device=device)
+            y_pred_test = y_pred_test.reshape(-1, Y.shape[-1])
+            varexp_per_pt[k,0] = ve_test      
+            varexp_per_pt[k,1] = compute_varexp(bin1d(Y[itest.flatten()], 4).flatten(), 
+                                                bin1d(y_pred_test, 4).flatten())
+            spks_pred_test = y_pred_test @ U.T
+            spks_test = spks[:,itest.flatten()].T
+            varexp_neurons_per_pt[:,k,0] = compute_varexp(spks_test, spks_pred_test)
+            spks_test_bin = bin1d(spks_test, 4)
+            spks_pred_test_bin = bin1d(spks_pred_test, 4)
+            varexp_neurons_per_pt[:,k,1] = compute_varexp(spks_test_bin, spks_pred_test_bin)
+            print(f'{k}, varexp {ve_test:.3f}, {varexp_neurons_per_pt[:,k,0].mean():.3f}')
+            return varexp, varexp_neurons, spks_pred_test0, itest, varexp_per_pt, varexp_neurons_per_pt
+    else:
+        return varexp, varexp_neurons, spks_pred_test0, itest, model
+
+class Core(nn.Module):
+    """ linear -> conv1d -> relu -> linear -> relu = latents for KPN model"""
+    def __init__(self, n_in=28, n_kp=None, n_filt=10, kernel_size=201, 
+                 n_layers=1, n_med=50, n_latents=256, 
+                 identity=False, same_conv=True, 
+                 relu_wavelets=True, relu_latents=True):
+        super().__init__()
+        self.n_in = n_in
+        self.n_kp = n_in if n_kp is None or identity else n_kp
+        self.n_filt = (n_filt//2) * 2 # must be even for initialization
+        self.relu_latents = relu_latents
+        self.relu_wavelets = relu_wavelets
+        self.same_conv = same_conv
+        self.n_layers = n_layers
+        self.n_latents = n_latents
+        self.features = nn.Sequential()
+
+        # combine keypoints into n_kp features
+        if identity:
+            self.features.add_module('linear0', nn.Identity(self.n_in))
+        else:
+            self.features.add_module('linear0', nn.Sequential(nn.Linear(self.n_in, self.n_kp),
+                                                              ))
+        # initialize filters with gabors
+        f = np.geomspace(1, 10, self.n_filt//2).astype('float32')
+        gw0 = gabor_wavelet(1, f[:,np.newaxis], 0, n_pts=kernel_size)
+        gw1 = gabor_wavelet(1, f[:,np.newaxis], np.pi/2, n_pts=kernel_size)
+        if self.same_conv:
+            # compute n_filt wavelet features of each one => n_filt * n_kp features
+            self.features.add_module('wavelet0', nn.Conv1d(1, self.n_filt, kernel_size=kernel_size,
+                                                        padding=kernel_size//2, bias=False))
+            self.features[-1].weight.data = torch.from_numpy(np.vstack((gw0, gw1))).unsqueeze(1)
+        else:
+            self.features.add_module('wavelet0', nn.Conv1d(self.n_kp, self.n_kp, kernel_size=kernel_size,
+                                                        padding=kernel_size//2, bias=False, groups=self.n_kp))
+            self.features[-1].weight.data = torch.tile(torch.from_numpy(gw0[[1]]).unsqueeze(1), 
+                                                        (self.n_kp, 1, 1))
+            self.n_filt = 1
+        for n in range(1, n_layers):
+            n_in = self.n_kp * self.n_filt if n==1 else n_med
+            self.features.add_module(f'linear{n}', nn.Sequential(nn.Linear(n_in, 
+                                                                            n_med),
+                                                                 ))
+
+        # latent linear layer
+        if self.n_latents > 0:
+            n_med = n_med if n_layers > 1 else self.n_filt * self.n_kp
+            self.features.add_module('latent', nn.Sequential(nn.Linear(n_med, n_latents),
+                                                        ))
+        
+    def wavelets(self, x):
+        """ compute wavelets of keypoints through linear + conv1d + relu layer """
+        # x is (n_batches, time, features)
+        out = self.features[0](x.reshape(-1, x.shape[-1]))
+        out = out.reshape(x.shape[0], x.shape[1], -1).transpose(2,1)
+        # out is now (n_batches, n_kp, time)
+        if self.same_conv:
+            out = out.reshape(-1, out.shape[-1]).unsqueeze(1)
+            # out is now (n_batches * n_kp, 1, time)
+            out = self.features[1](out)
+            # out is now (n_batches * n_kp, n_filt, time)
+            out = out.reshape(-1, self.n_kp * self.n_filt, out.shape[-1]).transpose(2,1)
+            out = out.reshape(-1, self.n_kp * self.n_filt)
+        else:
+            out = self.features[1](out)
+            out = out.transpose(-1,-2)
+        if self.relu_wavelets:
+            out = F.relu(out)
+        
+        # if n_layers > 1, go through more linear layers
+        for n in range(1, self.n_layers):
+            out = self.features[n+1](out)
+            out = F.relu(out)
+        return out
+                                              
+    def forward(self, x=None, wavelets=None):
+        """ x is (n_batches, time, features)
+            sample_inds is (sub_time) over batches
+        """
+        if wavelets is None:
+            wavelets = self.wavelets(x)
+        wavelets = wavelets.reshape(-1, wavelets.shape[-1])
+        
+        # latent layer
+        if self.n_latents > 0:
+            latents = self.features[-1](wavelets)
+            latents = latents.reshape(x.shape[0], -1, latents.shape[-1])
+            if self.relu_latents:
+                latents = F.relu(latents)
+            latents = latents.reshape(-1, latents.shape[-1])
+            return latents
+        else:
+            return wavelets
+
+class Readout(nn.Module):
+    """ linear layer from latents to neural PCs or neurons """
+    def __init__(self, n_animals=1, n_latents=256, n_layers=1, 
+                n_med=128, n_out=128):
+        super().__init__()
+        self.n_animals = n_animals
+        self.linear = nn.Sequential()
+        self.bias = nn.Parameter(torch.zeros(n_out))
+        if n_animals==1:
+            for j in range(n_layers):
+                n_in = n_latents if j==0 else n_med 
+                n_outc = n_out if j==n_layers-1 else n_med 
+                self.linear.append(nn.Linear(n_in, n_outc))
+                if n_layers > 1 and j < n_layers-1:
+                    self.linear.append(nn.ReLU())
+        else:
+            # no option for n_layers > 1
+            for n in range(n_animals):
+                self.linear.append(nn.Linear(n_latents, n_out))
+        self.bias.requires_grad = False
+
+    def forward(self, latents, animal_id=0):
+        if self.n_animals==1:
+            return self.linear(latents) + self.bias
+        else:
+            return self.linear[animal_id](latents) + self.bias
+
+class PredictionNetwork(nn.Module):
+    """ predict from behavior to neural PCs / neural activity model """
+    def __init__(self, n_in=28, n_kp=None, n_filt=10, kernel_size=201, n_core_layers=2,
+                 n_latents=256, n_out_layers=1, n_out=128, n_med=50, n_animals=1, same_conv=True,
+                 identity=False, relu_wavelets=True, relu_latents=True):
+        super().__init__()
+        self.core = Core(n_in=n_in, n_kp=n_kp, n_filt=n_filt, kernel_size=kernel_size, 
+                         n_layers=n_core_layers, n_med=n_med, n_latents=n_latents, same_conv=same_conv,
+                         identity=identity, relu_wavelets=relu_wavelets, relu_latents=relu_latents)
+        self.readout = Readout(n_animals=n_animals, 
+                               n_latents=n_latents if n_latents > 0 else n_filt*n_kp, 
+                               n_layers=n_out_layers, n_out=n_out)
+
+    def forward(self, x, sample_inds=None, animal_id=0):
+        latents = self.core(x)
+        if sample_inds is not None:
+            latents = latents[sample_inds]
+        latents = latents.reshape(x.shape[0], -1, latents.shape[-1])
+        y_pred = self.readout(latents, animal_id=animal_id)
+        return y_pred, latents
+    
+    def train_model(self, X_dat, Y_dat, tcam_list, tneural_list, 
+                        delay=-1, smoothing_penalty=0.5, 
+                    n_iter=300, learning_rate=1e-3, annealing_steps=2,
+                    weight_decay=1e-4, device=torch.device('cuda'), 
+                    split_time=False, verbose=False):
+        """ train behavior -> neural model using multiple animals """
+
+        optimizer = torch.optim.AdamW(self.parameters(), lr=learning_rate, weight_decay=weight_decay)
+        ### make input data a list if it's not already
+        not_list = False
+        if not isinstance(X_dat, list):
+            not_list = True
+            X_dat, Y_dat, tcam_list, tneural_list = [X_dat], [Y_dat], [tcam_list], [tneural_list]
+        
+        ### split data into train / test and concatenate
+        arrs = [[],[],[],[],[],[],[],[],[],[]]
+        for i, (X, Y, tcam, tneural) in enumerate(zip(X_dat, Y_dat, tcam_list, tneural_list)):
+            dsplits = split_data(X, Y, tcam, tneural, delay=delay, split_time=split_time, device=device)
+            for d,a in zip(dsplits, arrs):
+                a.append(d)
+        X_train, X_test, Y_train, Y_test, itrain_sample_b, itest_sample_b, itrain_sample, itest_sample, itrain, itest = arrs
+        n_animals = len(X_train)
+        
+        tic = time.time()
+        ### determine total number of batches across all animals to sample from
+        n_batches = [0]
+        n_batches.extend([X_train[i].shape[0] for i in range(n_animals)]) 
+        n_batches = np.array(n_batches)
+        c_batches = np.cumsum(n_batches)
+        n_batches = n_batches.sum()   
+
+        if n_iter > 199:
+            anneal_epochs = n_iter - 50*np.arange(1, annealing_steps+1)
+        else:
+            anneal_epochs = [-1]
+
+        ### optimize all parameters with SGD
+        for epoch in range(n_iter):
+            self.train()
+            if epoch in anneal_epochs:
+                if verbose:
+                    print('annealing learning rate')
+                optimizer.param_groups[0]['lr'] /= 10.
+            np.random.seed(epoch)
+            rperm = np.random.permutation(n_batches)
+            train_loss = 0
+            for nr in rperm:
+                i = np.nonzero(nr >= c_batches)[0][-1]
+                n = nr - c_batches[i]
+                y_pred = self.forward(X_train[i][n].unsqueeze(0), 
+                            itrain_sample_b[i][n], 
+                            animal_id=i)[0]
+                loss = ((y_pred - Y_train[i][n].unsqueeze(0))**2).mean()
+                loss += smoothing_penalty * (torch.diff(self.core.features[1].weight)**2).sum()
+                optimizer.zero_grad()
+                loss.backward()
+                optimizer.step()
+                train_loss += loss.item()
+                
+            train_loss /= n_batches
+
+            # compute test loss and test variance explained
+            if epoch%20==0 or epoch==n_iter-1:
+                ve_all, y_pred_all = [], []
+                self.eval()
+                with torch.no_grad():
+                    pstr = f'epoch {epoch}, '
+                    for i in range(n_animals):
+                        y_pred = self.forward(X_test[i], itest_sample_b[i].flatten(), animal_id=i)[0]
+                        y_pred = y_pred.reshape(-1, y_pred.shape[-1])
+                        tl = ((y_pred - Y_test[i])**2).mean()
+                        ve = 1 - tl / ((Y_test[i] - Y_test[i].mean(axis=0))**2).mean()
+                        y_pred_all.append(y_pred.cpu().numpy())
+                        ve_all.append(ve.item())
+                        if n_animals==1:
+                            pstr += f'animal {i}, train loss {train_loss:.4f}, test loss {tl.item():.4f}, varexp {ve.item():.4f}, '
+                        else:
+                            pstr += f'varexp{i} {ve.item():.4f}, '
+                pstr += f'time {time.time()-tic:.1f}s'
+                if verbose:
+                    print(pstr)
+        
+        if not_list:
+            return y_pred_all[0], ve_all[0], itest[0]
+        else:
+            return y_pred_all, ve_all, itest
+
+class MaxStimModel(nn.Module):
+    """ keypoint to neural PCs or activity model """
+    def __init__(self, model):
+        super().__init__()
+        self.model = model
+
+    def forward(self, x, u=None, sample_inds=None):
+        out = self.model(x, sample_inds)[0]
+        # out is neurons x 1 x n_out
+        if u is not None:
+            out = (out * u.unsqueeze(1)).sum(axis=-1)
+        return out 
+
+    def train_batch(self, u=None, learning_rate=1e-1, n_iter=200):
+        kernel_size = 2*self.model.core.features.wavelet0.kernel_size[0]
+        nf = self.model.core.n_in
+        device = self.model.core.features.wavelet0.weight.device
+        n_out = self.model.readout.linear[0].weight.shape[0]
+        nb = u.shape[0] if u is not None else n_out
+        # take a single timepoint from each batch
+        sample_inds = kernel_size * torch.from_numpy(np.arange(0,nb)).to(device) 
+        sample_inds += kernel_size//2
+        # each batch is a max stim
+        xr = 0.1 * torch.randn((nb, kernel_size, nf), device=device)
+        xr.requires_grad = True
+        optimizer = torch.optim.Adam([xr], lr=learning_rate, weight_decay=0)
+        for epoch in range(n_iter):
+            losses = 0
+            xr2 = xr / (1e-3 + (xr**2).mean(axis=(1,2), keepdims=True)**0.5)
+            y = self.forward(xr2, u=u, sample_inds=sample_inds)
+            loss = (-y).mean()
+            optimizer.zero_grad() 
+            loss.backward()
+            optimizer.step()
+            losses+=loss.item()
+            if epoch%50==0 or epoch==n_iter-1:
+                print(epoch, losses)
+        return xr2
+
+
+def train_model_test(model, X, Y, tcam, tneural, sgd=False, lam=1e-3, 
+                   n_iter=600, learning_rate=5e-4, fix_model=True,
+                   smoothing_penalty=1.0,
+                   weight_decay=1e-4, device=torch.device('cuda')):
+
+    dsplits = split_data(X, Y, tcam, tneural, device=device)
+    X_train, X_test, Y_train, Y_test, itrain_sample_b, itest_sample_b, itrain_sample, itest_sample, itrain, itest = dsplits
+            
+    tic = time.time()
+
+    n_batches = X_train.shape[0]
+    if sgd:
+        model.train()
+        if fix_model:
+            for param in model.parameters():
+                param.requires_grad = False 
+            model.test_classifier.weight.requires_grad = True
+            model.test_classifier.bias.requires_grad = True
+        else:
+            for param in model.parameters():
+                param.requires_grad = True 
+            
+        
+        optimizer = torch.optim.AdamW(model.parameters(), lr=learning_rate, weight_decay=weight_decay)
+        for epoch in range(n_iter):
+            model.train()
+            np.random.seed(epoch)
+            rperm = np.random.permutation(n_batches)
+            train_loss = 0
+            for n in rperm:
+                y_pred, latents = model(X_train[n].unsqueeze(0), 
+                                    itrain_sample_b[n], 
+                                    test=True)
+                loss = ((y_pred - Y_train[n].unsqueeze(0))**2).mean()
+                loss += smoothing_penalty * (torch.diff(model.features[1].weight)**2).sum()
+                optimizer.zero_grad()
+                loss.backward()
+                optimizer.step()
+                train_loss += loss.item()
+            train_loss /= n_batches
+            if epoch%20==0 or epoch==n_iter-1:
+                ve_all = []
+                y_pred_all = []
+                with torch.no_grad():
+                    model.eval()
+                    pstr = f'epoch {epoch}, '
+                    y_pred = model(X_test, itest_sample_b.flatten(), test=True)[0]
+                    tl = ((y_pred - Y_test)**2).mean()
+                    ve = 1 - tl / (Y_test**2).mean()
+                    #ve = ve.item()
+                    y_pred = y_pred.cpu().numpy()
+                    #y_pred_all.append(y_pred.cpu().numpy())
+                    #ve_all.append(ve.item())
+                    pstr += f'train loss {train_loss:.4f}, test loss {tl.item():.4f}, varexp {ve.item():.4f}'
+                    print(pstr)
+
+    else:
+        itrain = itrain.reshape(n_batches, -1)
+        l_train = itrain.shape[-1]
+        with torch.no_grad():
+            model.eval()
+            for n in range(n_batches):
+                y_pred, latents = model(X_train[n].unsqueeze(0), 
+                                    itrain_sample_b[n], 
+                                    test=True)
+                if n==0:
+                    n_latents = latents.shape[-1]
+                    latents_train = np.ones((itrain.size, n_latents+1), 'float32')
+                latents_train[n*l_train : (n+1)*l_train, :n_latents] = latents.cpu().numpy()
+            latents_test = np.ones((itest.size, n_latents+1), 'float32')
+            latents_test[:,:n_latents] = model(X_test, 
+                                            itest_sample_b.flatten(), 
+                                            test=True)[1].cpu().numpy().reshape(-1, n_latents)
+
+            Y_train = Y_train.cpu().numpy()
+            Y_test = Y_test.cpu().numpy().reshape(-1, Y_test.shape[-1])
+            Y_train = Y_train.reshape(-1, Y_train.shape[-1])          
+            A = np.linalg.solve(latents_train.T @ latents_train + lam * np.eye(n_latents+1),
+                                latents_train.T @ Y_train)
+            y_pred = latents_test @ A 
+            tl = ((y_pred - Y_test)**2).mean()
+            ve = 1 - tl / (Y_test**2).mean()
+            model.test_classifier.weight.data = torch.from_numpy(A[:n_latents].T).float().to(device)
+            model.test_classifier.bias.data = torch.from_numpy(A[-1]).float().to(device)
+            print(ve)
+
+    return y_pred, ve, itest
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `neuropop-0.1/neuropop/peer_prediction.py` & `neuropop-1.0/neuropop/peer_prediction.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,27 +1,30 @@
-import numpy as np 
-from neuropop.linear_prediction import linear_prediction
-
-def peer_prediction(spks, xpos, ypos, dum=400, tbin=4):
-    ineu1 = np.logical_xor((xpos%dum)<dum/2 , (ypos%dum) < dum/2)
-    #ineu1 = np.random.rand(len(spks)) > 0.5
-    ineu2 = np.logical_not(ineu1)
-    n_components = 128
-    Vn = []
-    for ineu in [ineu1, ineu2]:
-        Vn.append(PCA(n_components=n_components, copy=False).fit_transform(spks[ineu].T))
-    varexp = np.zeros(2)
-    varexp_neurons = np.zeros((spks.shape[0], 2))
-    for k,ineu in enumerate([ineu1, ineu2]):
-        V_pred_test,varexpk,itest = linear_prediction(Vn[(k+1)%2], Vn[k%2], rank=128, lam=1e-1, tbin=tbin)[:3]
-        varexp += varexpk[-1]
-        U = spks[ineu] @ Vn[k]
-        U /= (U**2).sum(axis=0)**0.5
-        spks_pred_test = V_pred_test @ U.T
-        spks_test = spks[ineu][:,itest].T
-        varexp_neurons[ineu, 0] = compute_varexp(spks_test, spks_pred_test)
-        spks_test_bin = bin1d(spks_test, tbin)
-        spks_pred_test_bin = bin1d(spks_pred_test, tbin)
-        varexp_neurons[ineu, 1] = compute_varexp(spks_test_bin, spks_pred_test_bin)
-    # average variance explained for two halves
-    varexp /= 2
+"""
+Copright © 2023 Howard Hughes Medical Institute, Authored by Carsen Stringer and Marius Pachitariu.
+"""
+import numpy as np 
+from neuropop.linear_prediction import linear_prediction
+
+def peer_prediction(spks, xpos, ypos, dum=400, tbin=4):
+    ineu1 = np.logical_xor((xpos%dum)<dum/2 , (ypos%dum) < dum/2)
+    #ineu1 = np.random.rand(len(spks)) > 0.5
+    ineu2 = np.logical_not(ineu1)
+    n_components = 128
+    Vn = []
+    for ineu in [ineu1, ineu2]:
+        Vn.append(PCA(n_components=n_components, copy=False).fit_transform(spks[ineu].T))
+    varexp = np.zeros(2)
+    varexp_neurons = np.zeros((spks.shape[0], 2))
+    for k,ineu in enumerate([ineu1, ineu2]):
+        V_pred_test,varexpk,itest = linear_prediction(Vn[(k+1)%2], Vn[k%2], rank=128, lam=1e-1, tbin=tbin)[:3]
+        varexp += varexpk[-1]
+        U = spks[ineu] @ Vn[k]
+        U /= (U**2).sum(axis=0)**0.5
+        spks_pred_test = V_pred_test @ U.T
+        spks_test = spks[ineu][:,itest].T
+        varexp_neurons[ineu, 0] = compute_varexp(spks_test, spks_pred_test)
+        spks_test_bin = bin1d(spks_test, tbin)
+        spks_pred_test_bin = bin1d(spks_pred_test, tbin)
+        varexp_neurons[ineu, 1] = compute_varexp(spks_test_bin, spks_pred_test_bin)
+    # average variance explained for two halves
+    varexp /= 2
     return varexp, varexp_neurons
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `neuropop-0.1/neuropop/split_data.py` & `neuropop-1.0/neuropop/split_data.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,149 +1,153 @@
-import numpy as np 
-import torch
-
-def split_traintest(n_t, frac=0.25, pad=3, split_time=False):
-    """this returns deterministic split of train and test in time chunks
-    
-    Parameters
-    ----------
-    n_t : int
-        number of timepoints to split
-    frac : float (optional, default 0.25)
-        fraction of points to put in test set
-    pad : int (optional, default 3)
-        number of timepoints to exclude from test set before and after training segment
-    split_time : bool (optional, default False)
-        split train and test into beginning and end of experiment
-    Returns
-    --------
-    itrain: 2D int array
-        times in train set, arranged in chunks
-    
-    itest: 2D int array
-        times in test set, arranged in chunks
-    """
-    #usu want 20 segs, but might not have enough frames for that
-    n_segs = int(min(20, n_t/4)) 
-    n_len = int(np.floor(n_t/n_segs))
-    inds_train = np.linspace(0, n_t - n_len - 5, n_segs).astype(int)
-    if not split_time:
-        l_train = int(np.floor(n_len * (1-frac)))
-        inds_test = inds_train + l_train + pad
-        l_test = np.diff(np.stack((inds_train, inds_train + l_train)).T.flatten()).min() - pad
-    else:
-        inds_test = inds_train[:int(np.floor(n_segs*frac))]
-        inds_train = inds_train[int(np.floor(n_segs*frac)):]
-        l_train = n_len - 10
-        l_test = l_train
-    itrain = (inds_train[:,np.newaxis] + np.arange(0, l_train, 1, int))
-    itest = (inds_test[:,np.newaxis] + np.arange(0, l_test, 1, int))
-    return itrain, itest
-
-
-def split_batches(tcam, tneural, frac=0.25, pad=3, split_time=False,
-                  itrain=None, itest=None):
-    """this returns deterministic split of train and test in time chunks for neural and cam times
-    
-    Parameters
-    ----------
-    n_t : int
-        number of timepoints to split
-    tcam : 1D array
-        times of camera frames
-    tneural : 1D array
-        times of neural frames
-    frac : float (optional, default 0.25)
-        fraction of points to put in test set
-    pad : int (optional, default 3)
-        number of timepoints to exclude from test set before and after training segment
-    split_time : bool (optional, default False)
-        split train and test into beginning and end of experiment
-    itrain: 2D int array
-        times in train set, arranged in chunks
-    
-    itest: 2D int array
-        times in test set, arranged in chunks
-    
-    Returns
-    --------
-    itrain: 1D int array
-        times in train set, arranged in chunks
-    
-    itest: 1D int array
-        times in test set, arranged in chunks
-    itrain_cam: 2D int array
-        times in cam frames in train set, arranged in chunks
-    itest_cam: 2D int array
-        times in cam frames in test set, arranged in chunks
-    """
-    
-    if itrain is None or itest is None:
-        itrain, itest = split_traintest(len(tneural), frac=frac, pad=pad, split_time=split_time)
-    inds_train, inds_test = itrain[:,0], itest[:,0]
-    l_train, l_test = itrain.shape[-1], itest.shape[-1]
-    
-    # find itrain and itest in cam inds
-    f = interp1d(tcam, np.arange(0, len(tcam)), kind='nearest', axis=-1,
-                fill_value='extrapolate', bounds_error=False)
-
-    inds_cam_train = f(tneural[inds_train]).astype('int')
-    inds_cam_test = f(tneural[inds_test]).astype('int')
-
-    l_cam_train = int(np.ceil(np.diff(tneural).mean() / np.diff(tcam).mean() * l_train))
-    l_cam_test = int(np.ceil(np.diff(tneural).mean() / np.diff(tcam).mean() * l_test))
-
-    # create itrain and itest in cam inds
-    itrain_cam = (inds_cam_train[:,np.newaxis] + np.arange(0, l_cam_train, 1, int))
-    itest_cam = (inds_cam_test[:,np.newaxis] + np.arange(0, l_cam_test, 1, int))
-    
-    itrain_cam = np.minimum(len(tcam)-1, itrain_cam)
-    itest_cam = np.minimum(len(tcam)-1, itest_cam)
-
-    # inds for downsampling itrain_cam and itest_cam
-    itrain_sample = f(tneural[itrain.flatten()]).astype(int)
-    itest_sample = f(tneural[itest.flatten()]).astype(int)
-    
-    # convert to indices in itrain_cam and itest_cam
-    it = np.zeros(len(tcam), 'bool')
-    it[itrain_sample] = True
-    itrain_sample = it[itrain_cam.flatten()].nonzero()[0]
-    
-    it = np.zeros(len(tcam), 'bool')
-    it[itest_sample] = True
-    itest_sample = it[itest_cam.flatten()].nonzero()[0]
-
-    return itrain, itest, itrain_cam, itest_cam, itrain_sample, itest_sample
-
-def split_data(X, Y, tcam, tneural, frac=0.25, delay=-1, split_time=False, device=torch.device('cuda')):
-    # ensure keypoints and timestamps are same length
-    tc, ttot = len(tcam), len(X)
-    inds = np.linspace(0, max(ttot,tc)-1, min(ttot,tc)).astype(int)
-    X = X[inds] if ttot > tc else X 
-    tcam = tcam[inds] if tc > ttot else tcam
-    if delay < 0:
-        Ys = np.vstack((Y[-delay:], np.tile(Y[[-1],:], (-delay,1))))
-        Xs = X
-    elif delay > 0:
-        Xs = np.vstack((X[delay:], np.tile(X[[-1],:], (delay,1))))
-        Ys = Y
-    else:
-        Xs = X 
-        Ys = Y
-    splits = split_batches(tcam, tneural, frac=frac, 
-                            split_time=split_time)
-    itrain, itest, itrain_cam, itest_cam, itrain_sample, itest_sample = splits
-    X_train = torch.from_numpy(Xs[itrain_cam]).float().to(device)
-    Y_train = torch.from_numpy(Ys[itrain]).float().to(device)
-    X_test = torch.from_numpy(Xs[itest_cam]).float().to(device)
-    Y_test = torch.from_numpy(Ys[itest]).float().to(device).reshape(-1, Y.shape[-1])
-    
-    itrain_sample_b = torch.zeros(itrain_cam.size, dtype=bool, device=device)
-    itrain_sample_b[itrain_sample] = True
-    itest_sample_b = torch.zeros(itest_cam.size, dtype=bool, device=device)
-    itest_sample_b[itest_sample] = True
-    itrain_sample_b = itrain_sample_b.reshape(itrain_cam.shape)
-    itest_sample_b = itest_sample_b.reshape(itest_cam.shape)
-    
-    itest -= delay
-
-    return X_train, X_test, Y_train, Y_test, itrain_sample_b, itest_sample_b, itrain_sample, itest_sample, itrain, itest
+"""
+Copright © 2023 Howard Hughes Medical Institute, Authored by Carsen Stringer and Marius Pachitariu.
+"""
+import numpy as np 
+from scipy.interpolate import interp1d
+import torch
+
+def split_traintest(n_t, frac=0.25, pad=3, split_time=False):
+    """this returns deterministic split of train and test in time chunks
+    
+    Parameters
+    ----------
+    n_t : int
+        number of timepoints to split
+    frac : float (optional, default 0.25)
+        fraction of points to put in test set
+    pad : int (optional, default 3)
+        number of timepoints to exclude from test set before and after training segment
+    split_time : bool (optional, default False)
+        split train and test into beginning and end of experiment
+    Returns
+    --------
+    itrain: 2D int array
+        times in train set, arranged in chunks
+    
+    itest: 2D int array
+        times in test set, arranged in chunks
+    """
+    #usu want 10 segs, but might not have enough frames for that
+    n_segs = int(min(10, n_t/4)) 
+    n_len = int(np.floor(n_t/n_segs))
+    inds_train = np.linspace(0, n_t - n_len - 5, n_segs).astype(int)
+    if not split_time:
+        l_train = int(np.floor(n_len * (1-frac)))
+        inds_test = inds_train + l_train + pad
+        l_test = np.diff(np.stack((inds_train, inds_train + l_train)).T.flatten()).min() - pad
+    else:
+        inds_test = inds_train[:int(np.floor(n_segs*frac))]
+        inds_train = inds_train[int(np.floor(n_segs*frac)):]
+        l_train = n_len - 10
+        l_test = l_train
+    itrain = (inds_train[:,np.newaxis] + np.arange(0, l_train, 1, int))
+    itest = (inds_test[:,np.newaxis] + np.arange(0, l_test, 1, int))
+    return itrain, itest
+
+
+def split_batches(tcam, tneural, frac=0.25, pad=3, split_time=False,
+                  itrain=None, itest=None):
+    """this returns deterministic split of train and test in time chunks for neural and cam times
+    
+    Parameters
+    ----------
+    n_t : int
+        number of timepoints to split
+    tcam : 1D array
+        times of camera frames
+    tneural : 1D array
+        times of neural frames
+    frac : float (optional, default 0.25)
+        fraction of points to put in test set
+    pad : int (optional, default 3)
+        number of timepoints to exclude from test set before and after training segment
+    split_time : bool (optional, default False)
+        split train and test into beginning and end of experiment
+    itrain: 2D int array
+        times in train set, arranged in chunks
+    
+    itest: 2D int array
+        times in test set, arranged in chunks
+    
+    Returns
+    --------
+    itrain: 1D int array
+        times in train set, arranged in chunks
+    
+    itest: 1D int array
+        times in test set, arranged in chunks
+    itrain_cam: 2D int array
+        times in cam frames in train set, arranged in chunks
+    itest_cam: 2D int array
+        times in cam frames in test set, arranged in chunks
+    """
+    
+    if itrain is None or itest is None:
+        itrain, itest = split_traintest(len(tneural), frac=frac, pad=pad, split_time=split_time)
+    inds_train, inds_test = itrain[:,0], itest[:,0]
+    l_train, l_test = itrain.shape[-1], itest.shape[-1]
+    
+    # find itrain and itest in cam inds
+    f = interp1d(tcam, np.arange(0, len(tcam)), kind='nearest', axis=-1,
+                fill_value='extrapolate', bounds_error=False)
+
+    inds_cam_train = f(tneural[inds_train]).astype('int')
+    inds_cam_test = f(tneural[inds_test]).astype('int')
+
+    l_cam_train = int(np.ceil(np.diff(tneural).mean() / np.diff(tcam).mean() * l_train))
+    l_cam_test = int(np.ceil(np.diff(tneural).mean() / np.diff(tcam).mean() * l_test))
+
+    # create itrain and itest in cam inds
+    itrain_cam = (inds_cam_train[:,np.newaxis] + np.arange(0, l_cam_train, 1, int))
+    itest_cam = (inds_cam_test[:,np.newaxis] + np.arange(0, l_cam_test, 1, int))
+    
+    itrain_cam = np.minimum(len(tcam)-1, itrain_cam)
+    itest_cam = np.minimum(len(tcam)-1, itest_cam)
+
+    # inds for downsampling itrain_cam and itest_cam
+    itrain_sample = f(tneural[itrain.flatten()]).astype(int)
+    itest_sample = f(tneural[itest.flatten()]).astype(int)
+    
+    # convert to indices in itrain_cam and itest_cam
+    it = np.zeros(len(tcam), 'bool')
+    it[itrain_sample] = True
+    itrain_sample = it[itrain_cam.flatten()].nonzero()[0]
+    
+    it = np.zeros(len(tcam), 'bool')
+    it[itest_sample] = True
+    itest_sample = it[itest_cam.flatten()].nonzero()[0]
+
+    return itrain, itest, itrain_cam, itest_cam, itrain_sample, itest_sample
+
+def split_data(X, Y, tcam, tneural, frac=0.25, delay=-1, split_time=False, device=torch.device('cuda')):
+    # ensure keypoints and timestamps are same length
+    tc, ttot = len(tcam), len(X)
+    inds = np.linspace(0, max(ttot,tc)-1, min(ttot,tc)).astype(int)
+    X = X[inds] if ttot > tc else X 
+    tcam = tcam[inds] if tc > ttot else tcam
+    if delay < 0:
+        Ys = np.vstack((Y[-delay:], np.tile(Y[[-1],:], (-delay,1))))
+        Xs = X
+    elif delay > 0:
+        Xs = np.vstack((X[delay:], np.tile(X[[-1],:], (delay,1))))
+        Ys = Y
+    else:
+        Xs = X 
+        Ys = Y
+    splits = split_batches(tcam, tneural, frac=frac, 
+                            split_time=split_time)
+    itrain, itest, itrain_cam, itest_cam, itrain_sample, itest_sample = splits
+    X_train = torch.from_numpy(Xs[itrain_cam]).float().to(device)
+    Y_train = torch.from_numpy(Ys[itrain]).float().to(device)
+    X_test = torch.from_numpy(Xs[itest_cam]).float().to(device)
+    Y_test = torch.from_numpy(Ys[itest]).float().to(device).reshape(-1, Y.shape[-1])
+    
+    itrain_sample_b = torch.zeros(itrain_cam.size, dtype=bool, device=device)
+    itrain_sample_b[itrain_sample] = True
+    itest_sample_b = torch.zeros(itest_cam.size, dtype=bool, device=device)
+    itest_sample_b[itest_sample] = True
+    itrain_sample_b = itrain_sample_b.reshape(itrain_cam.shape)
+    itest_sample_b = itest_sample_b.reshape(itest_cam.shape)
+    
+    itest -= delay
+
+    return X_train, X_test, Y_train, Y_test, itrain_sample_b, itest_sample_b, itrain_sample, itest_sample, itrain, itest
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `neuropop-0.1/neuropop/utils.py` & `neuropop-1.0/neuropop/utils.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,98 +1,100 @@
-import cv2
-import numpy as np
-from scipy.interpolate import interp1d
-from scipy.linalg import eigh
-from scipy.ndimage import gaussian_filter1d
-
-def bin1d(X, bin_size, axis=0):
-    """ mean bin over axis of data with bin bin_size """
-    if bin_size > 0:
-        size = list(X.shape)
-        Xb = X.swapaxes(0, axis)
-        Xb = Xb[:size[axis]//bin_size*bin_size].reshape((size[axis]//bin_size, bin_size, -1)).mean(axis=1)
-        Xb = Xb.swapaxes(axis, 0)
-        size[axis] = Xb.shape[axis]
-        Xb = Xb.reshape(size)
-        return Xb
-    else:
-        return X
-    
-def compute_varexp(y_true, y_pred):
-    """ variance explained of y_true by y_pred across axis=0
-    
-    """
-    y_var = ((y_true - y_true.mean(axis=0)) ** 2).mean(axis=0)
-    residual = ((y_true - y_pred) ** 2).mean(axis=0)
-    varexp = 1 - residual / y_var
-    return varexp 
-
-def resample_frames(data, torig, tout):
-    """
-    Resample data from times torig at times tout.
-    data is (n_samples, n_features). The data is filtered using a gaussian filter before resampling.
-    
-    Parameters
-    ----------
-    data : 2D array, input data (n_samples, n_features)
-    torig : 1D-array, original times
-    tout : 1D-array, times to resample to
-    Returns
-    --------
-    dout : ND-array
-        data resampled at tout
-    """
-    fs = torig.size / tout.size  # relative sampling rate
-    data = gaussian_filter1d(data, np.ceil(fs / 4), axis=0)
-    f = interp1d(torig, data, kind="linear", axis=0, fill_value="extrapolate")
-    dout = f(tout)
-    return dout
-
-def resample_data(data, tcam, tneural, crop='linspace'):
-    """
-    Resample data from camera times tcam at times tneural
-    sometimes there are fewer camera timestamps than frames, so data is cropped
-    data is (n_samples, n_features). The data is filtered using a gaussian filter before resampling.
-    
-    Parameters
-    ----------
-    data : 2D array, input data (n_samples, n_features)
-    tcam : 1D-array, original times
-    tneural : 1D-array, times to resample to
-    Returns
-    --------
-    data_resampled : ND-array
-        data resampled at tout
-    """
-    ttot = len(data)
-    tc = len(tcam)
-    if crop=='end':
-        d = data[:tc]
-    elif crop=='start':
-        d = data[ttot-tc:]
-    elif crop=='linspace':
-        d = data[np.linspace(0,ttot-1, tc).astype(int)]
-    else:
-        d = data[(ttot-tc)//2:(ttot-tc)//2+tc]
-    data_resampled = resample_frames(d, tcam, tneural)
-    return data_resampled
-
-
-def KLDiv_discrete(P, Q, binsize=200):
-    # Q is the null distribution; P and Q are 2D distributions
-    
-    x_bins = np.append(np.arange(0, np.amax(P[:,0]), binsize), np.amax(P[:,0]))
-    y_bins = np.append(np.arange(0, np.amax(P[:,1]), binsize), np.amax(P[:,1]))
-
-    this_KL = 0
-    for i in range(len(x_bins)-1):
-        for j in range(len(y_bins)-1):
-            Qx = (np.sum((Q[:,0] >= x_bins[i]) & (Q[:,0] < x_bins[i+1]) & \
-                        (Q[:,1] >= y_bins[j]) & (Q[:,1] < y_bins[j+1]))) / len(Q)
-            Px = (np.sum((P[:,0] >= x_bins[i]) & (P[:,0] < x_bins[i+1]) & \
-                        (P[:,1] >= y_bins[j]) & (P[:,1] < y_bins[j+1]))) / len(P)
-            if (Px == 0) | (Qx == 0): # no points in test or null distrib -- can't have log(0), or /0
-                continue
-
-            this_KL += Px * np.log(Px / Qx)
-    
-    return this_KL
+"""
+Copright © 2023 Howard Hughes Medical Institute, Authored by Carsen Stringer and Marius Pachitariu.
+"""
+import numpy as np
+from scipy.interpolate import interp1d
+from scipy.linalg import eigh
+from scipy.ndimage import gaussian_filter1d
+
+def bin1d(X, bin_size, axis=0):
+    """ mean bin over axis of data with bin bin_size """
+    if bin_size > 0:
+        size = list(X.shape)
+        Xb = X.swapaxes(0, axis)
+        Xb = Xb[:size[axis]//bin_size*bin_size].reshape((size[axis]//bin_size, bin_size, -1)).mean(axis=1)
+        Xb = Xb.swapaxes(axis, 0)
+        size[axis] = Xb.shape[axis]
+        Xb = Xb.reshape(size)
+        return Xb
+    else:
+        return X
+    
+def compute_varexp(y_true, y_pred):
+    """ variance explained of y_true by y_pred across axis=0
+    
+    """
+    y_var = ((y_true - y_true.mean(axis=0)) ** 2).mean(axis=0)
+    residual = ((y_true - y_pred) ** 2).mean(axis=0)
+    varexp = 1 - residual / y_var
+    return varexp 
+
+def resample_frames(data, torig, tout):
+    """
+    Resample data from times torig at times tout.
+    data is (n_samples, n_features). The data is filtered using a gaussian filter before resampling.
+    
+    Parameters
+    ----------
+    data : 2D array, input data (n_samples, n_features)
+    torig : 1D-array, original times
+    tout : 1D-array, times to resample to
+    Returns
+    --------
+    dout : ND-array
+        data resampled at tout
+    """
+    fs = torig.size / tout.size  # relative sampling rate
+    data = gaussian_filter1d(data, np.ceil(fs / 4), axis=0)
+    f = interp1d(torig, data, kind="linear", axis=0, fill_value="extrapolate")
+    dout = f(tout)
+    return dout
+
+def resample_data(data, tcam, tneural, crop='linspace'):
+    """
+    Resample data from camera times tcam at times tneural
+    sometimes there are fewer camera timestamps than frames, so data is cropped
+    data is (n_samples, n_features). The data is filtered using a gaussian filter before resampling.
+    
+    Parameters
+    ----------
+    data : 2D array, input data (n_samples, n_features)
+    tcam : 1D-array, original times
+    tneural : 1D-array, times to resample to
+    Returns
+    --------
+    data_resampled : ND-array
+        data resampled at tout
+    """
+    ttot = len(data)
+    tc = len(tcam)
+    if crop=='end':
+        d = data[:tc]
+    elif crop=='start':
+        d = data[ttot-tc:]
+    elif crop=='linspace':
+        d = data[np.linspace(0,ttot-1, tc).astype(int)]
+    else:
+        d = data[(ttot-tc)//2:(ttot-tc)//2+tc]
+    data_resampled = resample_frames(d, tcam, tneural)
+    return data_resampled
+
+
+def KLDiv_discrete(P, Q, binsize=200):
+    # Q is the null distribution; P and Q are 2D distributions
+    
+    x_bins = np.append(np.arange(0, np.amax(P[:,0]), binsize), np.amax(P[:,0]))
+    y_bins = np.append(np.arange(0, np.amax(P[:,1]), binsize), np.amax(P[:,1]))
+
+    this_KL = 0
+    for i in range(len(x_bins)-1):
+        for j in range(len(y_bins)-1):
+            Qx = (np.sum((Q[:,0] >= x_bins[i]) & (Q[:,0] < x_bins[i+1]) & \
+                        (Q[:,1] >= y_bins[j]) & (Q[:,1] < y_bins[j+1]))) / len(Q)
+            Px = (np.sum((P[:,0] >= x_bins[i]) & (P[:,0] < x_bins[i+1]) & \
+                        (P[:,1] >= y_bins[j]) & (P[:,1] < y_bins[j+1]))) / len(P)
+            if (Px == 0) | (Qx == 0): # no points in test or null distrib -- can't have log(0), or /0
+                continue
+
+            this_KL += Px * np.log(Px / Qx)
+    
+    return this_KL
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```


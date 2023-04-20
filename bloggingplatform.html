<?php

// Include the database configuration file
include 'config.php';

// Start the session
session_start();

// Check if the user is logged in
if (!isset($_SESSION['user_id'])) {
    header('Location: login.php');
    exit;
}

// Get the user's ID
$user_id = $_SESSION['user_id'];

// Handle form submissions
if ($_SERVER['REQUEST_METHOD'] == 'POST') {
    // Insert the new blog post into the database
    $title = $_POST['title'];
    $content = $_POST['content'];
    $category = $_POST['category'];
    $tags = $_POST['tags'];
    $sql = "INSERT INTO blog_posts (title, content, category, tags, user_id)
            VALUES ('$title', '$content', '$category', '$tags', $user_id)";
    mysqli_query($conn, $sql);
}

// Fetch the user's blog posts
$sql = "SELECT * FROM blog_posts WHERE user_id = $user_id ORDER BY created_at DESC";
$result = mysqli_query($conn, $sql);

?>

<html>
<head>
    <title>My Blog</title>
</head>
<body>
    <h1>Welcome to my blog, <?php echo $_SESSION['username']; ?>!</h1>

    <h2>Create a new post</h2>
    <form method="post">
        <label for="title">Title:</label>
        <input type="text" name="title"><br>
        <label for="content">Content:</label>
        <textarea name="content"></textarea><br>
        <label for="category">Category:</label>
        <input type="text" name="category"><br>
        <label for="tags">Tags:</label>
        <input type="text" name="tags"><br>
        <input type="submit" value="Submit">
    </form>

    <h2>My posts</h2>
    <?php while ($row = mysqli_fetch_assoc($result)): ?>
        <h3><?php echo $row['title']; ?></h3>
        <p><?php echo $row['content']; ?></p>
        <p>Category: <?php echo $row['category']; ?></p>
        <p>Tags: <?php echo $row['tags']; ?></p>
        <p>Created at: <?php echo $row['created_at']; ?></p>
        <hr>
    <?php endwhile; ?>
</body>
</html>

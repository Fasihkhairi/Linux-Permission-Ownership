# Create two users, user1 and user2
sudo useradd user1
sudo useradd user2

# Switch to user1
su user1

# Create a directory named devops9 and add file1.txt and file2.txt
mkdir devops9
touch devops9/file1.txt
touch devops9/file2.txt

# Run ls -al | grep devops9
ls -al | grep devops9

# This should show the contents of the devops9 directory.

# Run chmod +t devops9
chmod +t devops9

# Run ls -al | grep devops9 again
ls -al | grep devops9

# This should show that the sticky bit (+t) has been set on the devops9 directory.

# Switch to user2
su user2

# Change directory to devops9
cd devops9

# Delete file1.txt
rm file1.txt

# This will delete file1.txt from the devops9 directory.

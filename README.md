# Multiple Camera Post processing

Example of post processing with Main camera and UI camera

UI Camera has post processing that had blue colour grading.  If the UI Camera uses Clear Flags Depth the post processing effects the main camera image too. 

To Fix this the UI camera uses  Clear Flags with a solid colour with 0 transparency and a Render texture. The Render texture can then drawn using a canvas with a Screen overlay.
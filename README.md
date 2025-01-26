# Pocketpay
import { Card, CardContent } from "@/components/ui/card";
import { Button } from "@/components/ui/button";
import { Input } from "@/components/ui/input";
import { motion } from "framer-motion";

export default function KidsFinanceLandingPage() {
  return (
    <div className="min-h-screen bg-gradient-to-r from-blue-500 to-purple-500 p-6 text-white">
      <motion.h1
        className="text-4xl font-bold text-center mb-6"
        initial={{ opacity: 0, y: -50 }}
        animate={{ opacity: 1, y: 0 }}
      >
        Manage Your Pocket Money Smartly
      </motion.h1>

      <div className="max-w-4xl mx-auto grid grid-cols-1 md:grid-cols-2 gap-6">
        <Card className="p-6 bg-white text-black rounded-2xl shadow-lg">
          <CardContent>
            <h2 className="text-2xl font-semibold mb-2">Financial Literacy</h2>
            <p>Learn how to budget, save, and invest smartly with our engaging courses.</p>
          </CardContent>
        </Card>
        <Card className="p-6 bg-white text-black rounded-2xl shadow-lg">
          <CardContent>
            <h2 className="text-2xl font-semibold mb-2">Smart Investments</h2>
            <p>Explore different saving and investment options tailored for kids and teens.</p>
          </CardContent>
        </Card>
      </div>

      <div className="text-center mt-12">
        <h3 className="text-2xl font-semibold">Sign Up for Early Access</h3>
        <div className="mt-4 flex justify-center gap-4">
          <Input placeholder="Enter your email" className="w-80 p-3 rounded-lg text-black" />
          <Button className="bg-white text-blue-600 font-semibold p-3 rounded-lg">Join Now</Button>
        </div>
      </div>
    </div>
  );
}
